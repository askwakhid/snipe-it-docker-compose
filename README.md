# Snipe-IT Docker Compose

[Snipe-IT](https://snipeitapp.com/) is a free open source IT asset/license management system.

## Disclaimer
This is my development setup. I'm not responsible for any damages you may cause.

<h2 id="quickstart">⚡️ Initial Setup</h2>
1. Clone Repository
```bash 
git clone https://github.com/askwakhid/snipe-it-docker-compose.git 
```

2. Edit the .env file as per your requirement.

3. Run Snipe-IT docker-compose.yml
```bash
docker-compose up -d
```

4. Generate API Key
```bash
docker exec -it your-snipe-container sh
php artisan key:generate --show
```

5. Go to your .env file and replace {{INSERT_API_TOKEN}} with your API Key

6. Restart docker container
```bash
docker-compose down && docker-compose up -d --build 
```
7. Access Snipe-IT from your browser at :
```bash
http://127.0.0.1:3002
```