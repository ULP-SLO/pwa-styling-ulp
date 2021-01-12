ffUpscale

custom-component.component.ts [178]
				if (event.type === CustomComponentEventType.NAVIGATE) {
					for(const i in localStorage){
						if(i.substring(0,13) == "originOrderId" || i == "guest-customer-session-id" || i == "session-tracker"){
							localStorage.removeItem(i);
						}			
					}
					this.onNavigate(event as CustomComponentNavigationEvent);
					window.location.assign("/")
				}



style.sccs[17]
	background-color: white;


add-to-cart-button.component.html[8]
<i class="material-icons"
	*ngIf="!buttonText && !showAnimation">shopping_cart</i>