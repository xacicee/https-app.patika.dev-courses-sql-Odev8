# https-app.patika.dev-courses-sql-Odev8

--test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
CREATE TABLE employee(
   id INTEGER ,
   name VARCHAR(50), 
   birthday DATE, 
   email VARCHAR(100)
)
--Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
INSERT INTO employee (name, birthday, email)
VALUES
  ('Sherm','1980-10-11','svauls0@plala.or.jp'),
  ('Annadiane','1980-11-10','aperree2@exblog.jp'),
  ('Uta','1980-10-11','uhassell3@dedecms.com'),
  ('Frederique','1960-05-17','fdenny4@bloomberg.com'),
  ('Janel','1977-12-18','jkettlewell5@cafepress.com'),	
  ('Mersey','1919-01-20','msailor6@cbslocal.com'),
  ('Fee','1934-12-24','ftinn7@netlog.com'),
  ('Sioux','1972-12-10','sstaneland8@smh.com.au'),
  ('Duff','1970-12-10','dpischel9@google.com.br'),
  ('Robb','1917-10-14','rgiffena@oakley.com'),
  ('Aila','1950-12-25','agosdinb@macromedia.com'),
  ('Pansy','1960-10-10','pbeacomc@biglobe.ne.jp'),	
  ('Rivi','1980-10-12','rbarenskied@hostgator.com'),	
  ('Mariya','1960-12-12','mjiruseke@deviantart.com'),	
  ('Cassius','1972-10-14','colczykf@mlb.com'),	
  ('Ruthann','1980-04-12','rcatmullg@altervista.org'),
  ('Cammy','1982-12-13', 'ccossinsh@weibo.com'),
  ('Elaine','1982-12-13','ewasbroughi@storify.com'),
  ('Aleda','1982-12-13','agrimestonej@redcross.org'),	
  ('Morie','1982-12-13','mninnolik@t.com'),	
  ('Dulci','1982-12-13','dsnipel@economist.com'),	
  ('Eadith'	,'1982-12-13','epetrollim@fotki.com'),	
  ('Akim','1982-12-13','aoffinn@mapy.cz'),	
  ('Lisha','1982-12-13','lbemroseo@blogs.com'),	
  ('Francois','1982-12-13','fkobpacp@smh.com.au'),	 
  ('Philomena','1982-12-13','pyoungloves@geocities.com'),	
  ('Romonda','1982-12-13','rdjurisict@mail.ru'),	
  ('Marcella','1982-12-13','mbremeyeru@wufoo.com'),	
  ('Jodie','1982-12-13','jbaldelliv@tuttocitta.it'),	
  ('Nikolos','1982-12-13','ntrudgionx@wikispaces.com'),	
  ('Beaufort','1982-12-13','bflowerdewy@pinterest.com'),
  ('Randie','1982-12-13','rjahnerz@blogger.com'),
  ('Niels','1982-12-13','ngrube10@state.tx.uz'),	
  ('Konstantine','1982-12-13','kpero11@oakley.com'),
  ('Sallie','1982-12-13','sphilips12@youtube.com'),	
  ('Sondra','1982-12-13','sphorsby13@geocities.jp'),
  ('Modesta','1982-12-13','mcastanyer14@jiathis.com'),
  ('Harmonia','1982-12-13','hhacon15@skyrock.com'),	
  ('Sissy','1982-12-13','sdarrel16@youku.com'),	
  ('Deidre','1982-12-13','dgosney17@rambler.ru'),
  ('Llewellyn','1982-12-13','lpersehouse18@answers.com'),
  ('Ettore','1982-12-13','emylan19@comcast.net'),
  ('Melody','1982-12-13','mwilber1a@bing.com'),
  ('Lou','1982-12-13','lpedrol1b@washington.edu'),
  ('Arabel','1982-12-13','asherrott1c@ibm.com'),	
  ('Paola','1982-12-13','pfoakes1d@ed.gov'),	
  ('Theodosia','1982-12-13','tflott1e@comcast.net'),
  ('Davina','1982-12-13','dfrancescuccio1f@deliciousdays.com'),
  ('Win','1982-12-13','wwestrope1g@cyberchimps.com'),
  ('Ulric','1982-12-13','ukolinsky1h@arizona.edu'),
  ('Kate','1965-10-18','kate@nwrs.net');

--Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.  
UPDATE employee
SET name='hakan',
    birthday='1982-12-13',
	  email='hakan@gmail.com'
WHERE name='M%';

UPDATE employee
SET name='ali',
    birthday='1992-11-13',
    email='ali@gmail.com'
WHERE like name='%t';

UPDATE employee
SET birthday='1984-12-30'
WHERE name='katy';

UPDATE employee
SET name='mary'
WHERE id=2;

UPDATE employee
SET name='kerim'
WHERE id=12;

--Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
DELETE FROM employee
WHERE name='katy';

DELETE FROM employee
WHERE id=3;

DELETE FROM employee
WHERE id=9;

DELETE FROM employee
WHERE id>48;

DELETE FROM employee
WHERE name='hakan';
