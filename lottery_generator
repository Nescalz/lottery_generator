from PyQt5.QtCore import Qt
from PyQt5.QtWidgets import QApplication, QWidget, QPushButton, QLabel, QVBoxLayout
from random import randint
pop = 1
def kn():
    global pop 
    rand = randint(1, 9)
    rand2 = randint(1, 9)
    winer.setText(str(rand))
    winer2.setText(str(rand2))
    if rand == rand2:
        text.setText(str(pop))
        pop = 1
    else:
        text.setText("You lost")
        pop += 1

app = QApplication([])
main_win = QWidget()
main_win.resize(400, 200)

main_win.setWindowTitle("Lottery")
button = QPushButton("Try")
text = QLabel("Goo")
winer = QLabel("?")
winer2 = QLabel("?")

line = QVBoxLayout()
line.addWidget(text ,alignment=Qt.AlignCenter)
line.addWidget(winer,alignment=Qt.AlignCenter)
line.addWidget(winer2,alignment=Qt.AlignCenter)
line.addWidget(button,alignment=Qt.AlignCenter)
main_win.setLayout(line)

button.clicked.connect(kn)

main_win.show()
app.exec_()
