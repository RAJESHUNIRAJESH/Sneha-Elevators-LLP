# Sneha-Elevators-LLP

series = str(input("Enter series RM,VL,SL : "))
width = int(input("Enter Shaft width : "))
depth = int(input("Enter Shaft depth : "))
plastering = str(input("Enter w or wo or oo : "))
counter = str(input("Enter sc or bc : "))
opening = str(input("Enter t or c : "))                # for SL series only t (telescopic)

if plastering == 'wo':
  width -= 60
  depth -= 50
elif plastering == 'oo':
  width -= 100
  depth -= 100

if series == 'RM':
  if counter == 'sc':
    if opening == 't':
      width -= 580
      depth -= 400
    else:
      width -= 580
      depth -= 340
  else:
    if opening == 't':
      width -= 380
      depth -= 600
    else:
      width -= 380
      depth -= 540

elif series == 'VL':
  if counter == 'sc':
    if opening == 't':
      width -= 580
      depth -= 400
    else:
      width -= 580
      depth -= 340
  else:
    if opening == 't':
      width -= 380
      depth -= 600
    else:
      width -= 380
      depth -= 540

elif series == 'SL':
  if counter == 'sc':
    width -= 570
    depth -= 410
  else:
    width -= 220
    depth -= 760

print("Cabin Width :",width)
print("Cabin Depth :",depth)
