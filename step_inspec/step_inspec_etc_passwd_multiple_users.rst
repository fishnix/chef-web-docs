.. This is an included how-to. 

.. To test for multiple root users:

.. code-block:: ruby

   describe passwd.uid(0) do
     its('username') { should eq 'root' }
     its('count') { should eq 1 }
   end

   describe passwd.uid(33) do
     its('username') { should eq 'www-data' }
     its('count') { should eq 1 }
   end
