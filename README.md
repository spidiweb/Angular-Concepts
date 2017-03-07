# Angular-Concepts

Create event  and Emit it.

var Appearance_FilterClicked = $rootScope.$on('Appearance_FilterClicked', function (event, Appearance_Filter) {
        $scope.LoadDataWithFilter(Appearance_Filter)
    });
	
	
	
	$rootScope.$emit('Appearance_FilterClicked', {
            SuitFilter: $('#hdnAppearancesSearchSuits').val(),
            FirmFilter: $('#hdnAppearancesSearchFirms').val(),
            FromDate: appearanceSearchFromDate,
            ToDate: appearanceSearchToDate
        });
		
