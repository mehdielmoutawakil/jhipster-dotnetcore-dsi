# Introduction 
Jhipster dotnetcore code generator

# Getting Started

## 1. Installation process

### Step 1: Set Up Your JHipster Development Environment
Ensure you have JHipster installed globally: ` npm install -g yo generator-jhipster `

### Step 2: Clone jhipster dotnetcore custom generator repository
` https://dsi-cs@dev.azure.com/dsi-cs/CodeGen/_git/Back-DotNetCore `

### Step 3: Link jhipster dotnetcore custom generator repository
` npm link `

### Step 4: Create new jhipster dotnetcore project
jhipster --blueprints dotnetcore --skip-client --skip-checks

### Step 5: Generate migration files 
` add-migration InitialCreate `

### Step 6: Update appsettings ConnextionStrings
` "AppDbContext": "Data Source=.;Initial Catalog=jhipster;Integrated Security=True;Trusted_Connection=True;MultipleActiveResultSets=true;TrustServerCertificate=True;" `

### Step 7: Install migrations
` update-database `

### Step8: import JDL file
` jhipster import-jdl <jdlfilepath> `