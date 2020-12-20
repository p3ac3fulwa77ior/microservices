# Microservices Project Make File

VIRTUALENV = $(shell)

clean: shutdown
	rm -fr microservices.egg-info
	rm -fr venv

venv:
	$(VIRTUALENV) 

install: clean venv
	 python setup.py install
	 python setup.py develop

launch: venv shutdown
	
	
	 python  bookings.py &
	

shutdown:

	ps -ef | grep "bookings.py" | grep -v grep | awk '{print $$2}' | xargs --no-run-if-empty kill 
