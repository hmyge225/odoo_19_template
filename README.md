## Etape 1:
    docker-compose up -d --build

## Etape 2 (Crée DB via UI):
    Ouvre http://localhost:8071
    Manage Databases → Master pass :
        Create Database
        Name: mycompany
        Email: admin@mycompany.com
        Password: admin123
        Langue: Français
        Pays: France
        Create

## Etape 3 (Vérifie qifparse):
    docker-compose exec web python3 -c "import qifparse; print('qifparse OK')"

--------------------------------------------------------------------------------
## NB : --Notions Utiles-- 
    
    1. Supprime TOUT:
        docker-compose down -v --remove-orphans
        docker system prune -a --volumes -f
