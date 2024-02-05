class Member:
    def __init__(self, m_code, name, address, phone, fc1=None, fc2=None, fc3=None):
        self.m_code = m_code
        self.name = name
        self.address = address
        self.phone = phone
        self.fc1 = fc1
        self.fc2 = fc2
        self.fc3 = fc3

    def display_member_info(self):
        print(f"Member Code: {self.m_code}")
        print(f"Member Name: {self.name}")
        print(f"Address: {self.address}")
        print(f"Phone Number: {self.phone}")
        print(f"Facility Code 1: {self.fc1}")
        print(f"Facility Code 2: {self.fc2}")
        print(f"Facility Code 3: {self.fc3}")
        print()


def main():
    members = []

    
    member1 = Member(1, "ARUSHA", "W-45, P.BAGH, NEW DELHI", 5454789, 1, 1, 1)
    member2 = Member(2, "YAMAN", "Z-55, R.L.COLONY, DELHI", 2121345, 1, 1)
    member3 = Member(3, "RAJAN", "S-9/2, TARA APPTS, DELHI", 4689920, 1)

    members.extend([member1, member2, member3])

    
    for member in members:
        member.display_member_info()

if __name__ == "__main__":
    main()



