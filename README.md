arduinoInterface

usage:
$ python
>> from arduinoInterface import arduinoInterface
>> a = arduinoInterface() #(port=None, baud=9600, cycle_delay=0.01)
>> #defaults to auto-finding first available port
>> a.writeln('hi Arduino')
>> a.write('new data')
>> a.read()
>> #returns text from Arduino and possibly waiting for transmission completion due to clock speed differences
>> a.close() #be kind.. and rewind.
>> a.open(self, port='COM1', baud=9600) #specify particular port
>> a.clearBuf() #clear internal string buffer (not pending port values)