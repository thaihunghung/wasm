(func $func252 (param $var0 i32) (result i32)
    local.get $var0
    i32.const 255
    i32.and
    i32.const 91424
    i32.add
    i32.load8_u
    local.get $var0
    i32.const 16
    i32.shr_u
    i32.const 255
    i32.and
    i32.const 91424
    i32.add
    i32.load8_u
    i32.const 16
    i32.shl
    local.get $var0
    i32.const 24
    i32.shr_u
    i32.const 91424
    i32.add
    i32.load8_u
    i32.const 24
    i32.shl
    i32.or
    local.get $var0
    i32.const 8
    i32.shr_u
    i32.const 255
    i32.and
    i32.const 91424
    i32.add
    i32.load8_u
    i32.const 8
    i32.shl
    i32.or
    i32.or
  )

  (func $func202 (param $var0 i32) (param $var1 i32) (result i32)
    local.get $var1
    i32.const 4
    i32.ge_u
    if
      local.get $var0
      i32.load align=1
      local.tee $var0
      i32.const 24
      i32.shl
      local.get $var0
      i32.const 65280
      i32.and
      i32.const 8
      i32.shl
      i32.or
      local.get $var0
      i32.const 8
      i32.shr_u
      i32.const 65280
      i32.and
      local.get $var0
      i32.const 24
      i32.shr_u
      i32.or
      i32.or
      return
    end
    unreachable
  )
