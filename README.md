 -- Partie 4
-- 1
select * from client where nomcl like 'A%' and adrcl='tunis';
-- 2
select * from produit where pu > 300;
-- 3
select * from commande where datec = date'2023-10-22';
-- 4
select * from produit where qtes=null;
-- 5
select * from produit where lib like '%e';
-- 6
select * from categorie 
where substr(libcategorie, 3, 1) = 'a' and libcategorie like '%s';
-- 7
select * from client order by nomcl asc;
-- 8
select * from produit order by pu desc;
-- 9
select * from commande order by datec asc;
-- 10
select * from commande order by montantc desc;
-- 11
select count(*) from client;
-- 12
select avg(pu) from produit;
-- 13
select * from produit where pu > (select avg(pu) from produit);
-- 14
select sum(montantc) from commande;
-- 15
select avg(montantc) from commande;
-- 16
select count(*) from produit where qtes > 0;
-- 17
select * from produit where pu = (select min(pu) from produit);
-- 19
select stkmin from produit;
-- 20 
select * from produit where pu = (select max(pu) from produit);
