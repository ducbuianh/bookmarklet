# bookmarklet
Useful bookmarkler

[HRM Autofill Bookmarklet](javascript:(function(){var data=prompt("Enter data:"),reason=prompt("Enter reason:"),inputs=["working_date","old_start_time","old_end_time","reason"];if(null==data||""==data)alert("Hmmmm....");else{var lines=data.split(", ");lines.forEach((e,t)=>{var a=e.split(/[\s]+/);for(a.splice(1,1),a.push(reason),j=0;j<inputs.length;j++)document.querySelectorAll("input[id^="+inputs[j]+"]")[t].value=a[j];t<lines.length-1&&document.getElementById("addNewTimeShift").click()})}})();)
