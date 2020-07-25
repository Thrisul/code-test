Quote estimation for user given and customized cycle configuration

Steps to run the application
===============================
Step 1: Go to  CycleApp folder and run below steps to perform db setup
			> python manage.py makemigrations
			> python manage.py migrate
			> python manage.py runserver 8000

Step 2: Open browser/postman and run below url	
			http://127.0.0.1:8000/admin/

Step 3 :Give the configurations of cycle,in payload and send api call to backend as per requirement
				1. Tyres
				2. Wheels
				3. Seat
				4. Body
				5. chain
				6. Brakes
		And give below url
		http://127.0.0.1:8000/calc_cycle_configuration/
		API:
		====
		Suffix url :  /estimate_cycle_cost/
		Request method : POST
		Content-Type: application/json
		Payload : 
					[   {"tyres":2},
						{"wheels":2},
						{"brakes":3},
						{"seat":1},
						{"bell":1}
					]

