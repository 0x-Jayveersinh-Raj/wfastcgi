# wfastcgi
    <configuration>
  <system.webServer>
    <handlers>
      <add name="FlaskHandler"
           path="*"
           verb="*"
           modules="FastCgiModule"
           scriptProcessor="C:\Python311\python.exe|C:\Python311\Lib\site-packages\wfastcgi.py"
           resourceType="Unspecified" />
    </handlers>
  </system.webServer>

  <appSettings>
    <add key="WSGI_HANDLER" value="app.app" />
    <add key="PYTHONPATH" value="D:\Projects\MyFlaskAPI" />
  </appSettings>
</configuration>
