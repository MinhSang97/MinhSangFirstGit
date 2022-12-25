# MinhSangFirstGit
Project hoidanit
xampp 8.0.6
nodejs node-v14.17.0-x64
sequelize npm install --save-div sequelize-cli@6.6.2
cd src
npx sequelize-cli init
https://www.sharepointdiary.com/2014/03/fix-for-powershell-script-cannot-be-loaded-because-running-scripts-is-disabled-on-this-system.html

25/12 end #21 https://www.youtube.com/watch?v=B4sy3DL4IX0&list=PLncHg6Kn2JT6E38Z3kit9Hnif1xC_9VqI&index=30

👉 1. Cài đặt các thư viện: sequlize-cli, sequelize và mysql2
npm install --save-dev sequelize-cli@6.2.0
npm install --save mysql2@2.2.5
npm install --save sequelize@6.6.2

👉 2. Thêm file .sequelizerc tại thư mục root
Nội dung file .sequelizerc
const path = require('path');
module.exports = {
  'config': path.resolve('./src/config', 'config.json'),
  'migrations-path': path.resolve('./src', 'migrations'),
  'models-path': path.resolve('./src', 'models'),
  'seeders-path': path.resolve('./src', 'seeders')
}

👉 Tại thư mục root, sử dụng câu lệnh: node_modules/.bin/sequelize init

👉 3. Tạo model: 
npx sequelize-cli model:generate --name User --attributes firstName:string,lastName:string,email:string

👉 4: Tạo migrations:
npx sequelize-cli db:migrate

👉5. Tạo Seeder: npx sequelize-cli seed:generate --name demo-user



Github:

1. git init
2. git add .
3. git commit -m 'noi dung'
4. git remote add origin https://github.com/MinhSang97/MinhSangFirstGit.git (COPY GIT)
5. git push origin master 

sau khi thay doi:
1. git add .
2. git commit -m 'noi dung
3. git push origin master 
