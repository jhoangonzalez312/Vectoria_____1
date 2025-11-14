create database VECTORIA
use VECTORIA
create table REGISTRO(
    NOMBRE_USUARIO VARCHAR(30), 
	ID INT,
	NOMBRE VARCHAR(30),
	APELLIDO VARCHAR(30),
	GENERO VARCHAR(30),
	EDAD INT,
	GMAIL VARCHAR(50),
	CONTRASEÑA VARCHAR(30))

insert into	REGISTRO(NOMBRE_USUARIO,ID,NOMBRE,APELLIDO,GENERO,EDAD,GMAIL,CONTRASEÑA)
	values('hevert123',1,'clemente','taticuan','no binario',22,'hevertclemente123@gmail.com','teamoesteban123')
	

insert into REGISTRO(NOMBRE_USUARIO,ID,NOMBRE,APELLIDO,GENERO,EDAD,GMAIL,CONTRASEÑA) values
('ana_luna',2,'Ana','Luna','femenino',28,'ana.luna28@gmail.com','luna2025'),
('josemaria99',3,'José','María','masculino',35,'josemaria99@hotmail.com','clave123'),
('valquiriax',4,'Valquiria','Santos','no binario',30,'valquiriax@outlook.com','santosx30'),
('mauro_dev',5,'Mauro','González','masculino',26,'mauro.dev@gmail.com','devpass26'),
('carla_vega',6,'Carla','Vega','femenino',24,'carla.vega24@yahoo.com','vegacarla24'),
('leo_astro',7,'Leonardo','Astorga','masculino',31,'leo.astro@gmail.com','astroleo31'),
('dani_moon',8,'Daniela','Moon','femenino',29,'dani.moon29@gmail.com','moonlight29'),
('cris_fern',9,'Cristian','Fernández','masculino',33,'cris.fernandez@gmail.com','ferncris33'),
('alejandrax',10,'Alejandra','Ruiz','no binario',27,'alejandrax@live.com','ruizale27'),
('natalie_art',11,'Natalie','Arteaga','femenino',25,'natalie.art@gmail.com','arteaga25'),
('marco_polo',12,'Marco','Polo','masculino',34,'marco.polo34@gmail.com','polomarco34'),
('sofia_star',13,'Sofía','Estrella','femenino',22,'sofia.star22@gmail.com','estrella22'),
('raultech',14,'Raúl','Torres','masculino',36,'raultech@gmail.com','torresraul36'),
('vivian_zen',15,'Vivian','Zapata','femenino',32,'vivian.zen32@gmail.com','zenvivian32'),
('hevert123',1,'Clemente','Taticuan','no binario',22,'hevertclemente123@gmail.com','teamoesteban123')


select*from REGISTRO

DELETE FROM REGISTRO
WHERE ID = 1;

create table ESTADO(
ID INT,
NOMBRE_USUARIO VARCHAR(30),
PUNTAJE INT,
NIVEL_CUENTA int,
LOGROS_DESBLOQUEADOS INT)

INSERT INTO ESTADO(ID, NOMBRE_USUARIO, PUNTAJE, NIVEL_CUENTA, LOGROS_DESBLOQUEADOS) VALUES
(1, 'hevert123', 850, 72, 12),
(2, 'ana_luna', 920, 88, 15),
(3, 'josemaria99', 670, 54, 8),
(4, 'valquiriax', 740, 63, 10),
(5, 'mauro_dev', 810, 70, 11),
(6, 'carla_vega', 580, 39, 5),
(7, 'leo_astro', 990, 95, 17),
(8, 'dani_moon', 760, 66, 9),
(9, 'cris_fern', 690, 52, 7),
(10, 'alejandrax', 830, 75, 13),
(11, 'natalie_art', 610, 47, 6),
(12, 'marco_polo', 940, 91, 16),
(13, 'sofia_star', 550, 33, 4),
(14, 'raultech', 880, 80, 14),
(15, 'vivian_zen', 720, 60, 8)

select*from ESTADO, REGISTRO

create table INVENTARIO(
ID_ITEM INT,
NOMBRE_ITEM VARCHAR(30),
ID_USUARIO VARCHAR(30),
CANTIDAD INT,
FECHA_OBTENIDO INT)

INSERT INTO INVENTARIO(ID_ITEM, NOMBRE_ITEM, ID_USUARIO, CANTIDAD, FECHA_OBTENIDO) VALUES
(101, 'Espada de Fuego', 'hevert123', 1, 20231015),
(102, 'Poción Curativa', 'ana_luna', 5, 20230920),
(103, 'Escudo de Hierro', 'josemaria99', 2, 20230805),
(104, 'Cristal Mágico', 'valquiriax', 3, 20231101),
(105, 'Botas de Velocidad', 'mauro_dev', 1, 20231030),
(106, 'Mapa del Tesoro', 'carla_vega', 1, 20230718),
(107, 'Arco de Luz', 'leo_astro', 2, 20230925),
(108, 'Llave Dorada', 'dani_moon', 1, 20231010),
(109, 'Anillo de Poder', 'cris_fern', 1, 20230822),
(110, 'Pergamino Antiguo', 'alejandrax', 4, 20231103),
(111, 'Casco de Dragón', 'natalie_art', 1, 20230912),
(112, 'Gema Azul', 'marco_polo', 6, 20231005),
(113, 'Capa Invisible', 'sofia_star', 1, 20230730),
(114, 'Libro de Hechizos', 'raultech', 2, 20231106),
(115, 'Lanza Sagrada', 'vivian_zen', 1, 20230828);

select*from INVENTARIO

create table ESTADISTICAS(
ID_USUARI VARCHAR(30),
PARTIDAS_JUGADAS INT,
DAÑO_TOTAL INT,
TIEMPO_PROMEDIO_PARTIDA INT,
MUERTES INT)


INSERT INTO ESTADISTICAS(ID_USUARI, PARTIDAS_JUGADAS, DAÑO_TOTAL, TIEMPO_PROMEDIO_PARTIDA, MUERTES) VALUES
('hevert123', 120, 15800, 540, 34),
('ana_luna', 98, 13450, 480, 27),
('josemaria99', 76, 8900, 510, 22),
('valquiriax', 105, 12100, 495, 30),
('mauro_dev', 112, 14300, 530, 29),
('carla_vega', 64, 7200, 460, 18),
('leo_astro', 140, 17600, 550, 36),
('dani_moon', 88, 9700, 475, 24),
('cris_fern', 79, 8600, 490, 21),
('alejandrax', 110, 13900, 520, 28),
('natalie_art', 70, 8100, 470, 20),
('marco_polo', 130, 16500, 560, 33),
('sofia_star', 58, 6800, 450, 17),
('raultech', 125, 15200, 540, 31),
('vivian_zen', 92, 10100, 485, 25);

select*from ESTADISTICAS 


create table ECONOMIA(
ID_USUARIO VARCHAR(30),
TIPO_MONEDA VARCHAR(30),
SALDO_ACTUAL INT,
TRANSACCIONES VARCHAR(30))

INSERT INTO ECONOMIA(ID_USUARIO, TIPO_MONEDA, SALDO_ACTUAL, TRANSACCIONES) VALUES
('hevert123', 'Oro', 1500, 'Compra,Venta'),
('ana_luna', 'Gemas', 320, 'Recompensa,Intercambio'),
('josemaria99', 'Oro', 870, 'Compra,Donación'),
('valquiriax', 'Cristales', 540, 'Intercambio,Recompensa'),
('mauro_dev', 'Oro', 1200, 'Venta,Recompensa'),
('carla_vega', 'Gemas', 250, 'Compra,Intercambio'),
('leo_astro', 'Oro', 2000, 'Recompensa,Venta'),
('dani_moon', 'Cristales', 410, 'Intercambio,Compra'),
('cris_fern', 'Oro', 980, 'Donación,Venta'),
('alejandrax', 'Gemas', 600, 'Recompensa,Compra'),
('natalie_art', 'Cristales', 300, 'Intercambio,Donación'),
('marco_polo', 'Oro', 1750, 'Venta,Recompensa'),
('sofia_star', 'Gemas', 190, 'Compra,Intercambio'),
('raultech', 'Cristales', 720, 'Recompensa,Venta'),
('vivian_zen', 'Oro', 1100, 'Intercambio,Compra');

select*from REGISTRO


