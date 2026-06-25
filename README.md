# 1. นิยามคลาสสำหรับเก็บข้อมูลสถานที่ท่องเที่ยว
class TouristAttraction:
    # ฟังก์ชันเริ่มต้นสำหรับกำหนดค่าคุณสมบัติ (Attributes)
    def __init__(self, name, location, attraction_type, rating):
        self.name = name                 # ชื่อสถานที่
        self.location = location         # ที่ตั้ง/จังหวัด/ประเทศ
        self.attraction_type = attraction_type   # ประเภท (เช่น ทะเล, วัด, ภูเขา)
        self.rating = rating             # คะแนนรีวิว (เต็ม 5)

    # ฟังก์ชันพิเศษแสดงผลข้อมูลวัตถุเมื่อสั่ง print()
    def __str__(self):
        return f"{self.name} ({self.location})"

    # เมธอด (Method) แสดงรายละเอียดแบบเต็ม
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
# ทดสอบพิมพ์วัตถุตรงๆ (จะเรียกใช้ __str__)
print(my_trip) 

# เรียกใช้เมธอดเพื่อแสดงรายละเอียดทั้งหมด
my_trip.display_info()