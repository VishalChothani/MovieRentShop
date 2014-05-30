function validateBlank(field, alerttxt)
{
	if (field.value == null || field.value.trim() == "")
    {
    	alert(alerttxt);
		field.focus();
		return false;
    }
    else
    {
    	return true;
    }
}

function validateDropDown(field, fieldName)
{
	if (field.selectedIndex == 0)
	{
		alert('Please select ' + fieldName);
		field.focus();
		return false;
	}
	return true;
}

// only allow characters to be entered
function validateChar(field)
{
	var checkStr = field.value;
	var isOnlyCharacters = /^[a-zA-Z]+$/.test(checkStr);
	if(!isOnlyCharacters) {
		alert("Numbers and Special characters like '!,@,$,%,^,&,*' are not allowed");
		field.value="";
		field.focus();
	}
	return isOnlyCharacters;
}


//VALIDATES E-MAIL ID
function validateEmail(field, alerttxt)
{
	if (validateBlank(field,alerttxt)==false)
  	{
  		return false;
  	}
	
	with (field)
  	{
  		apos=value.indexOf("@");
  		dotpos=value.lastIndexOf(".");

  		if (apos<1||dotpos-apos<2)
    	{
    		alert("Incorrect Email Id");
			field.value="";
			field.focus();
    		return false;
    	}
  		else 
  		{
  			return true;
  		}
  	}
}

function validate(field,alerttxt)
{
	if (validateBlank(field,alerttxt)==false)
  	{
  		return false;
  	}
	
	if (validateChar(field)==false)
  	{
  		return false;
  	}
	return true;
}

/*function validatePassword(field, alerttxt)
{
	if (validateBlank(field, alerttxt)==false)
  	{
  		return false;
  	}	
	if (field.value.length < 6)
	{
		alert("Password must contain atleast 6 characters");
		field.value="";
		field.focus();
		return (false);
	}
	return true;
}*/

function validateBothPasswords(password1, password2)
{
	if (password1.value != password2.value)
	{
		alert("Passwords do not match");
		password2.value="";
		password1.value="";
		password1.focus();
		return false;
	}
	return true;
}

function validateNum(field)
{
	var checkStr = field.value;
	var isOnlyCharacters = /^[0-9]+$/.test(checkStr);
	if(!isOnlyCharacters) {
		alert("Characters and special characters '!,@,$,%,^,&,*' are not allowed");
		field.value="";
		field.focus();
	}
	return isOnlyCharacters;
}

function validateLength(field, length, alertTxt)
{
	if(field.value.length < length) {
		if(alertTxt == null) {
			alert("Please enter " + length + " digit number/text");
		} else {
			alert(alertTxt);
		}
		field.value="";
		field.focus();
		return false;
	}
	return true;
}

function validateSSN (value) {
	var isValidSSN = /^\d{3}-\d{2}-\d{4}$/.test(value);
	if (!isValidSSN) {
		alert("Not a valid SSN");
		return false;
	}
	return true;
}

function validateZIP (value) {
	var isValidZip = /(^\d{5}$)|(^\d{5}-\d{4}$)/.test(value);
	if (!isValidZip) {
		alert("Not a valid ZIP code");
		return false;
	}
	return true;
}

function setFocus(field)
{
	field.focus();
}