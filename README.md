Last login: Wed Apr 12 15:15:50 on ttys000
╭─    ~ ───────────────────────────────────────────── ✔  08:14:43 PM  ─╮
╰─ qmk compile -c -kb crkbd -km samalander                                   ─╯
QMK Firmware 0.18.8
Making crkbd/rev1 with keymap samalander and target clean

Ψ Compiling keymap with gmake --jobs=1 crkbd/rev1:samalander


QMK Firmware 0.18.8
Making crkbd/rev1 with keymap samalander

avr-gcc (Homebrew AVR GCC 8.5.0) 8.5.0
Copyright (C) 2018 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

Generating: .build/obj_crkbd_rev1/src/info_config.h                                                 [OK]
Generating: .build/obj_crkbd_rev1/src/default_keyboard.c                                            [OK]
Generating: .build/obj_crkbd_rev1/src/default_keyboard.h                                            [OK]
Generating: .build/obj_crkbd_rev1/src/layouts.h                                                     [OK]
Compiling: keyboards/crkbd/crkbd.c                                                                  [OK]
Compiling: keyboards/crkbd/rev1/rev1.c                                                              [OK]
Compiling: .build/obj_crkbd_rev1/src/default_keyboard.c                                             [OK]
Compiling: quantum/keymap_introspection.c                                                          In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:67:1: error: unknown type name 'tap_dance_action_t'; did you mean 'qk_tap_dance_action_t'?
 tap_dance_action_t tap_dance_actions[] = {
 ^~~~~~~~~~~~~~~~~~
 qk_tap_dance_action_t
./keyboards/crkbd/keymaps/samalander/keymap.c:67:20: error: conflicting types for 'tap_dance_actions'
 tap_dance_action_t tap_dance_actions[] = {
                    ^~~~~~~~~~~~~~~~~
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:78:30: note: previous declaration of 'tap_dance_actions' was here
 extern qk_tap_dance_action_t tap_dance_actions[];
                              ^~~~~~~~~~~~~~~~~
In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:69:5: error: braces around scalar initializer [-Werror]
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
     ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:5: note: (near initialization for 'tap_dance_actions[0]')
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:60:11: error: field name not in record or union initializer
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
           ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:11: note: (near initialization for 'tap_dance_actions[0]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
           ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:69:5: error: braces around scalar initializer [-Werror]
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
     ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:5: note: (near initialization for 'tap_dance_actions[0]')
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:60:18: error: initialization of 'int' from 'void (*)(qk_tap_dance_state_t *, void *)' {aka 'void (*)(struct <anonymous> *, void *)'} makes integer from pointer without a cast [-Werror=int-conversion]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:18: note: (near initialization for 'tap_dance_actions[0]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:49: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:49: note: (near initialization for 'tap_dance_actions[0]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:77: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                             ^~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:77: note: (near initialization for 'tap_dance_actions[0]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                             ^~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:103: error: field name not in record or union initializer
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                       ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:103: note: (near initialization for 'tap_dance_actions[0]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                       ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:116: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                                    ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:116: note: (near initialization for 'tap_dance_actions[0]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                                    ^
./keyboards/crkbd/keymaps/samalander/keymap.c:69:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_BRC] = ACTION_TAP_DANCE_DOUBLE(KC_LBRC, KC_RBRC),
                ^~~~~~~~~~~~~~~~~~~~~~~
In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:71:5: error: braces around scalar initializer [-Werror]
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
     ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:5: note: (near initialization for 'tap_dance_actions[1]')
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:60:11: error: field name not in record or union initializer
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
           ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:11: note: (near initialization for 'tap_dance_actions[1]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
           ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:71:5: error: braces around scalar initializer [-Werror]
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
     ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:5: note: (near initialization for 'tap_dance_actions[1]')
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:60:18: error: initialization of 'int' from 'void (*)(qk_tap_dance_state_t *, void *)' {aka 'void (*)(struct <anonymous> *, void *)'} makes integer from pointer without a cast [-Werror=int-conversion]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:18: note: (near initialization for 'tap_dance_actions[1]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:49: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:49: note: (near initialization for 'tap_dance_actions[1]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:77: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                             ^~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:77: note: (near initialization for 'tap_dance_actions[1]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                             ^~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:103: error: field name not in record or union initializer
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                       ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:103: note: (near initialization for 'tap_dance_actions[1]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                       ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:116: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                                    ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:116: note: (near initialization for 'tap_dance_actions[1]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                                    ^
./keyboards/crkbd/keymaps/samalander/keymap.c:71:15: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_QG] = ACTION_TAP_DANCE_DOUBLE(KC_QUOT, KC_GRV),
               ^~~~~~~~~~~~~~~~~~~~~~~
In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:73:5: error: braces around scalar initializer [-Werror]
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
     ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:5: note: (near initialization for 'tap_dance_actions[2]')
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:60:11: error: field name not in record or union initializer
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
           ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:11: note: (near initialization for 'tap_dance_actions[2]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
           ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
In file included from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:73:5: error: braces around scalar initializer [-Werror]
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
     ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:5: note: (near initialization for 'tap_dance_actions[2]')
In file included from quantum/quantum.h:120,
                 from keyboards/crkbd/rev1/rev1.h:22,
                 from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
quantum/process_keycode/process_tap_dance.h:60:18: error: initialization of 'int' from 'void (*)(qk_tap_dance_state_t *, void *)' {aka 'void (*)(struct <anonymous> *, void *)'} makes integer from pointer without a cast [-Werror=int-conversion]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:18: note: (near initialization for 'tap_dance_actions[2]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:49: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:49: note: (near initialization for 'tap_dance_actions[2]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:77: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                             ^~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:77: note: (near initialization for 'tap_dance_actions[2]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                             ^~~~~~~~~~~~~~~~~~~~~~~
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:103: error: field name not in record or union initializer
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                       ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:103: note: (near initialization for 'tap_dance_actions[2]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                       ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:116: error: excess elements in scalar initializer [-Werror]
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                                    ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
quantum/process_keycode/process_tap_dance.h:60:116: note: (near initialization for 'tap_dance_actions[2]')
         { .fn = {qk_tap_dance_pair_on_each_tap, qk_tap_dance_pair_finished, qk_tap_dance_pair_reset}, .user_data = (void *)&((qk_tap_dance_pair_t){kc1, kc2}), }
                                                                                                                    ^
./keyboards/crkbd/keymaps/samalander/keymap.c:73:16: note: in expansion of macro 'ACTION_TAP_DANCE_DOUBLE'
     [TD_PRN] = ACTION_TAP_DANCE_DOUBLE(KC_LPRN, KC_RPRN),
                ^~~~~~~~~~~~~~~~~~~~~~~
In file included from keyboards/crkbd/crkbd.h:21,
                 from ./keyboards/crkbd/keymaps/samalander/keymap.c:19,
                 from quantum/keymap_introspection.c:5:
./keyboards/crkbd/keymaps/samalander/keymap.c:87:127: error: 'CW_TOGG' undeclared here (not in a function); did you mean 'CL_TOGG'?
     XXXXXXX, KC_LGUI, KC_LALT, KC_LCTL, KC_LSFT, XXXXXXX,                        KC_CAPS, KC_LEFT, KC_DOWN, KC_UP,   KC_RGHT, CW_TOGG,
                                                                                                                               ^~~~~~~
keyboards/crkbd/rev1/rev1.h:37:7: note: in definition of macro 'LAYOUT_split_3x6_3'
     { R15, R14, R13, R12, R11, R10 }, \
       ^~~
cc1: all warnings being treated as errors
 [ERRORS]
 |
 |
 |
gmake[1]: *** [builddefs/common_rules.mk:359: .build/obj_crkbd_rev1_samalander/quantum/keymap_introspection.o] Error 1
gmake: *** [Makefile:414: crkbd/rev1:samalander] Error 1
Make finished with errors

╭─    ~ ──────────────────────────────────── 2 ✘  7s   08:15:16 PM  ─╮
╰─                                                                           ─╯

