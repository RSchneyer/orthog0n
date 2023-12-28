import board
dir(board)
from kmk.kmk_keyboard import KMKKeyboard
from kmk.keys import KC
from kmk.scanners import DiodeOrientation
from kmk.modules.layers import Layers

keyboard = KMKKeyboard()
keyboard.modules.append(Layers())
keyboard.col_pins = (board.A1, board.A0, board.SCK, board.MISO, board.MOSI, board.D10, board.D4, board.D3, board.D2, board.A2, board.A3, board.D1)
keyboard.row_pins = (board.D5, board.D6, board.D7, board.D8, board.D9,)
keyboard.diode_orientation = DiodeOrientation.COL2ROW

LAYER02 = KC.LT(2, KC.SPC)
LAYER03 = KC.LT(3, KC.SPC)
NAVLAYR = KC.MO(4)

keyboard.keymap = [
    # typing layer
    [
        KC.ESC,  KC.N1,   KC.N2,   KC.N3, KC.N4,  KC.N5, KC.NO,   KC.NO,   KC.NO,   KC.NO,  KC.NO,   KC.NO,\
        KC.TAB,  KC.Q,    KC.W,    KC.E,  KC.R,   KC.T,  KC.Y,    KC.U,    KC.I,    KC.O,   KC.P,    KC.BSPC,\
        KC.LCTL, KC.A,    KC.S,    KC.D,  KC.F,   KC.G,  KC.H,    KC.J,    KC.K,    KC.L,   KC.SCLN, KC.QUOT,\
        KC.LSFT, KC.Z,    KC.X,    KC.C,  KC.V,   KC.B,  KC.N,    KC.M,    KC.COMM, KC.DOT, KC.SLSH, KC.ENT,\
        KC.LCTL, KC.LWIN, KC.LALT, KC.NO, LAYER03, KC.NO, NAVLAYR, LAYER02, KC.NO,   KC.NO,  KC.NO,   KC.TG(1),
    ],
    # gaming layer
    [
        KC.ESC,  KC.N1,   KC.N2,   KC.N3, KC.N4,  KC.N5, KC.NO,   KC.NO,   KC.NO,   KC.NO,  KC.NO,   KC.NO,\
        KC.TAB,  KC.Q,    KC.W,    KC.E,  KC.R,   KC.T,  KC.Y,    KC.U,    KC.I,    KC.O,   KC.P,    KC.BSPC,\
        KC.LCTL, KC.A,    KC.S,    KC.D,  KC.F,   KC.G,  KC.H,    KC.J,    KC.K,    KC.L,   KC.SCLN, KC.QUOT,\
        KC.LSFT, KC.Z,    KC.X,    KC.C,  KC.V,   KC.B,  KC.N,    KC.M,    KC.COMM, KC.DOT, KC.SLSH, KC.ENT,\
        KC.LCTL, KC.ESC, KC.LALT, KC.NO, KC.SPC, KC.NO, NAVLAYR, LAYER02, KC.NO,   KC.NO,  KC.NO,   KC.TG(0),
    ],
    # numbers layer and -=[]\
    [
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.NO,   KC.NO,   KC.NO,   KC.NO,   KC.NO,   KC.NO,\
        KC.GRV,  KC.N1,   KC.N2,   KC.N3,   KC.N4,   KC.N5,   KC.N6,   KC.N7,   KC.N8,   KC.N9,   KC.N0,   KC.NO,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.MINS, KC.EQL,  KC.LBRC, KC.RBRC, KC.BSLS,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.LSFT, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS,
    ],
    # shifted numbers layer
    [
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.NO,   KC.NO,   KC.NO,   KC.NO,   KC.NO,   KC.NO,\
        KC.GRV,  KC.EXLM, KC.AT,   KC.HASH, KC.DLR,  KC.PERC, KC.CIRC, KC.AMPR, KC.ASTR, KC.LPRN, KC.RPRN, KC.NO,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.UNDS, KC.PLUS, KC.LCBR, KC.RCBR, KC.PIPE,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.LSFT, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS,
    ],
    # navigation + fkey layer
    [
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.NO,   KC.NO,   KC.NO,   KC.NO,   KC.NO,   KC.NO,\
        KC.TRNS, KC.F1,   KC.F2,   KC.F3,   KC.F4,   KC.TRNS, KC.TRNS, KC.TRNS, KC.UP,   KC.TRNS, KC.TRNS, KC.TRNS,\
        KC.CAPS, KC.F5,   KC.F6,   KC.F7,   KC.F8,   KC.TRNS, KC.TRNS, KC.LEFT, KC.DOWN, KC.RGHT, KC.TRNS, KC.TRNS,\
        KC.TRNS, KC.F9,   KC.F10,  KC.F11,  KC.F12,  KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS,\
        KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS, KC.TRNS,
    ]
]

if __name__ == '__main__':
    print('hello world!')
    keyboard.go()
