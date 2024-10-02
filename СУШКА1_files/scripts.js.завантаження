	$(document).ready(function() {
		
		/* scroll */
		
		$("a[href^='#']").click(function(){
			var _href = $(this).attr("href");
			$("html, body").animate({scrollTop: $(_href).offset().top+"px"});
			return false;
		});

		/* sliders */

		$(".owl-carousel").owlCarousel({
			items: 1,
			loop: true,
			smartSpeed: 300,
			mouseDrag: false,
			pullDrag: false,
			dots: false,
			nav: true,
			navText: ""
		});

		/* timer */

		/*function update() {
			var Now = new Date(), Finish = new Date();
			Finish.setHours( 23);
			Finish.setMinutes( 59);
			Finish.setSeconds( 59);
			if( Now.getHours() === 23  &&  Now.getMinutes() === 59  &&  Now.getSeconds === 59) {
				Finish.setDate( Finish.getDate() + 1);
			}
			var sec = Math.floor( ( Finish.getTime() - Now.getTime()) / 1000);
			var hrs = Math.floor( sec / 3600);
			sec -= hrs * 3600;
			var min = Math.floor( sec / 60);
			sec -= min * 60;
			$(".timer .hours").html( pad(hrs));
			$(".timer .minutes").html( pad(min));
			$(".timer .seconds").html( pad(sec));
			setTimeout( update, 200);
		}
		function pad(s) {
			s = ("00"+s).substr(-2);
			return "<span>" + s[0] + "</span><span>" + s[1] + "</span>";
		}
		update();*/
		
		 function update() {
			var Now = new Date(),
				Finish = new Date();
			Finish.setHours(23);
			Finish.setMinutes(59);
			Finish.setSeconds(59);
			// Если текущее время больше чем время окончания, установите Finish на следующий день
			if (Now > Finish) {
				Finish.setDate(Finish.getDate() + 1);
			}
			var sec = Math.floor((Finish.getTime() - Now.getTime()) / 1000);
			var hrs = Math.floor(sec / 3600);
			sec -= hrs * 3600;
			var min = Math.floor(sec / 60);
			sec -= min * 60;
			$(".timer .hours").text(pad(hrs));
			$(".timer .minutes").text(pad(min));
			$(".timer .seconds").text(pad(sec));
			setTimeout(update, 200);
		}

		function pad(s) {
			return ("00" + s).substr(-2);
		}

		update();
		
		/* validate form */

		$(".order_form").submit(function(){
			if ($(this).find("input[name='fio']").val() == "" && $(this).find("input[name='number']").val() == "") {
				alert("Введите ваши имя и телефон");
				$(this).find("input[name='fio']").focus();
				return false;
			}
			else if ($(this).find("input[name='fio']").val() == "") {
				alert("Введите ваше имя");
				$(this).find("input[name='fio']").focus();
				return false;
			}
			else if ($(this).find("input[name='number']").val() == "") {
				alert("Введите ваш телефон");
				$(this).find("input[name='number']").focus();
				return false;
			}
			return true;
		});


	});

	$(window).on("load", function(){
		$("#more_link_1").click(function(){
		  $("#more_link_1").hide();
		  $("#more_text_1").show();
		});
	});


