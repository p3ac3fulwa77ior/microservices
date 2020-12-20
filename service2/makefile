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
	
	
	 python  service2/bookings.py &
	

shutdown:

	ps -ef | grep "service2/bookings.py" | grep -v grep | awk '{print $$2}' | xargs --no-run-if-empty kill 
