# 1. นิยามคลาสสำหรับเก็บข้อมูลสถานที่ท่องเที่ยว
class TouristAttraction: 
    
    def __init__(self, name, location, attraction_type, rating):
        self.name = name              
        self.location = location         
        self.attraction_type = attraction_type   
        self.rating = rating          

    def __str__(self):
        return f"{self.name} ({self.location})"

    def display_info(self):
        print(f"--- ข้อมูลสถานที่ท่องเที่ยว ---")
        print(f"ชื่อสถานที่: {self.name}")
        print(f"ที่ตั้ง: {self.location}")
        print(f"ประเภท: {self.attraction_type}")
        print(f"คะแนนรีวิว: {self.rating} / 5 ดาว")


# 2. สร้างวัตถุ (Object) จากคลาสจำนวน 1 วัตถุ
my_trip = TouristAttraction(
    name="วัดพระแก้ว (วัดพระศรีรัตนศาสดาราม)", 
    location="กรุงเทพมหานคร, ประเทศไทย", 
    attraction_type="วัดและโบราณสถาน", 
    rating=4.9
)

# 3. ทดสอบเรียกใช้งานวัตถุ
print(my_trip) 
my_trip.display_info()
