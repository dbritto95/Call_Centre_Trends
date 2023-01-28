# Call_Centre_Trends
My first PWC Call Centre Trends Visualisation dashboard by the @virtual forage virtual internship programme 
# Measures created for the dashboard
% Total Abondened calls = [Total Abandoned Calls] / [Total Calls] # calulated the percentage

% Total answered calls = [Total Answered Calls] / [Total Calls] 

Average speed of answered Calls = AVERAGE('Call history'[Speed of answer in seconds])

Average Talk Duration = FORMAT(AVERAGE('Call history'[AvgTalkDuration]),"HH:NN:SS")

Total Abandoned Calls = COUNTAX(FILTER('Call history', [Answered (Y/N)] = "n"), [Answered (Y/N)])

Total Answered Calls = COUNTAX(FILTER('Call history',[Answered (Y/N)] = "Y"), [Answered (Y/N)])

Total Talk Duration = FORMAT(SUM('Call history'[AvgTalkDuration]), "HH:NN:SS")
