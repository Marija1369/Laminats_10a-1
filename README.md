# Laminats_10a-1

room_length = float(input("Ievadiet istabas garumu (m): "))

room_width = float(input("Ievadiet istabas platumu (m): "))

laminate_price = float(input("Ievadiet lamināta pakas cenu (EUR): "))

laminate_area_per_package = float(input("Ievadiet lamināta pakas sedzošo platību (m²): "))

board_length = float(input("Ievadiet plāksnes garumu (m): "))

board_width = float(input("Ievadiet plāksnes platumu (m): "))



room_area = room_length * room_width # Istabas platība m²

board_area = board_length * board_width # Vienas plāksnes platība m²


required_laminate_area = room_area * 1.10


packages_needed = (required_laminate_area / laminate_area_per_package)

packages_needed = round(packages_needed) # Noapaļošana uz augšu līdz veselam skaitlim


total_cost = packages_needed * laminate_price


print(f"Istabas platība ir {room_area:.2f} m².")

print(f"Lamināta platība ar rezervi: {required_laminate_area:.2f} m².")

print(f"Nepieciešamais lamināta paku skaits: {packages_needed}.")

print(f"Kopējās izmaksas: {total_cost:.2f} EUR.")
