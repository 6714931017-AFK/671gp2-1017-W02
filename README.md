# 1. นิยามคลาส (Class Definition)
class TouristAttraction:
    # ฟังก์ชันคอนสตรัคเตอร์ (__init__) สำหรับกำหนดคุณลักษณะ (Attributes) ของวัตถุ
    def __init__(self, name, location, attraction_type, highlight):
        self.name = name                 # ชื่อสถานที่
        self.location = location         # ที่ตั้ง/จังหวัด
        self.attraction_type = attraction_type # ประเภท (เช่น ทะเล, วัด, ภูเขา)
        self.highlight = highlight       # จุดเด่นสำคัญ

    # เมธอด (Method) สำหรับแสดงข้อมูลของสถานที่ท่องเที่ยว
    def display_info(self):
        print(f"--- ข้อมูลสถานที่ท่องเที่ยว ---")
        print(f"ชื่อสถานที่: {self.name}")
        print(f"ที่ตั้ง: {self.location}")
        print(f"ประเภท: {self.attraction_type}")
        print(f"จุดเด่น: {self.highlight}")
        print("-" * 30)

# 2. การสร้างวัตถุ (Object Creation) จากคลาส
# สร้างวัตถุชื่อ 'attraction1' และส่งค่าข้อมูลเข้าไป
attraction1 = TouristAttraction(
    name="วัดพระแก้ว (วัดพระศรีรัตนศาสดาราม)",
    location="กรุงเทพมหานคร",
    attraction_type="โบราณสถาน / วัดคู่บ้านคู่เมือง",
    highlight="ประดิษฐานพระพุทธมหามณีรัตนปฏิมากร และสถาปัตยกรรมไทยอันวิจิตรบรรจง"
)

# 3. การเรียกใช้งานเมธอดเพื่อแสดงผล
attraction1.display_info()
