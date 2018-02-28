# How to setting postgresql in Gekko

make sure you install postgresql and create db name 'gekko'

install pg:
npm install pg@6.1.0

cd gekko(where you install)

if you use UI

vi web/vue/UIconfig.js

adapter: 'sqlite'
modify
adapter: 'postgresql'

save file

then 

vi web/routes/baseConfig.js 

find
connectionString: 'postgres://user:pass@localhost:5432', // if default port

replace

connectionString: 'postgres://your_user:your_password@localhost:5432', // if default port

find

database: null,
replace
database: 'gekko'

save file

fin.
    
