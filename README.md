function Activities_OnLoad(executionContext){
	debugger;
	var formContext = executionContext.getFormContext();
	if(formContext.getAttribute("ownerid").getValue() != null){
		formContext.getControl("header_ownerid").setDisabled(true);
	}
	else{
	formContext.getControl("header_ownerid").setDisabled(false);
	}
}
