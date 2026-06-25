# 1. นิยามคลาส (Class Definition)
class TouristAttraction:
    # Constructor สำหรับกำหนดค่าเริ่มต้นของสถานที่ท่องเที่ยว
    def __init__(self, name, location, category, rating):
        self.name = name          # ชื่อสถานที่
        self.location = location  # ที่ตั้ง/จังหวัด
        self.category = category  # ประเภท (เช่น ทะเล, วัด, ภูเขา)
        self.rating = rating      # คะแนนรีวิว (เต็ม 5)

    # Method สำหรับแสดงข้อมูลของสถานที่ท่องเที่ยว
    def display_info(self):
        print(f"--- ข้อมูลสถานที่ท่องเที่ยว ---")
        print(f"ชื่อสถานที่: {self.name}")
        print(f"ที่ตั้ง: {self.location}")
        print(f"ประเภท: {self.category}")
        print(f"คะแนนรีวิว: {self.rating} / 5")
        
    # Method สำหรับจำลองการเช็คอิน
    def check_in(self):
        return f"📍 คุณได้เช็คอินที่ {self.name} เรียบร้อยแล้ว!"

# ---------------------------------------------------------

# 2. การสร้างวัตถุ (Object Creation)
attraction1 = TouristAttraction(
    name="วัดพระแก้ว (วัดพระศรีรัตนศาสดาราม)", 
    location="กรุงเทพมหานคร", 
    category="วัดและโบราณสถาน", 
    rating=4.9
)

# 3. เรียกใช้งาน Method ของวัตถุ
attraction1.display_info()
print(attraction1.check_in())