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

  (func $func250 (param $var0 i32) (param $var1 i32) (param $var2 i32) (param $var3 i32)
    (local $var4 i32)
    (local $var5 i32)
    (local $var6 i32)
    (local $var7 i32)
    (local $var8 i32)
    (local $var9 i32)
    (local $var10 i32)
    (local $var11 i32)
    (local $var12 i32)
    (local $var13 i32)
    (local $var14 i32)
    (local $var15 i32)
    (local $var16 i32)
    (local $var17 i32)
    (local $var18 i32)
    global.get $global0
    i32.const 48
    i32.sub
    local.tee $var9
    global.set $global0
    i32.const 177372
    i32.load
    local.set $var16
    i32.const 177372
    local.get $var9
    i32.const 24
    i32.add
    i32.store
    local.get $var9
    i32.const 8
    i32.add
    local.set $var11
    i32.const 484
    i32.const 3
    call $func36
    local.set $var6
    local.get $var1
    local.set $var7
    block $label3
      block $label0
        block $label2
          block $label1
            local.get $var2
            i32.const 16
            i32.sub
            local.tee $var1
            i32.const 16
            i32.gt_u
            i32.const 1
            local.get $var1
            i32.shl
            i32.const 65793
            i32.and
            i32.eqz
            i32.or
            i32.eqz
            if
              local.get $var6
              i32.eqz
              br_if $label0
              local.get $var2
              i32.const 32
              i32.ne
              if
                local.get $var2
                i32.const 24
                i32.eq
                if
                  i32.const 12
                  local.set $var4
                  br $label1
                end
                local.get $var2
                i32.const 16
                i32.ne
                br_if $label2
                i32.const 10
                local.set $var4
                br $label1
              end
              i32.const 14
              local.set $var4
              br $label1
            end
            i32.const 0
            local.set $var6
            i32.const 108568
            local.set $var4
            br $label3
          end $label1
          local.get $var6
          local.get $var4
          i32.store
        end $label2
        i32.const 0
        local.set $var4
        local.get $var2
        local.get $var3
        i32.gt_u
        local.set $var8
        local.get $var2
        i32.const 2
        i32.shr_u
        local.tee $var3
        local.set $var5
        local.get $var2
        local.set $var1
        loop $label10
          local.get $var5
          i32.eqz
          if
            local.get $var3
            local.get $var3
            local.get $var6
            i32.load
            local.tee $var8
            i32.const 2
            i32.shl
            local.tee $var12
            i32.const 4
            i32.add
            local.tee $var13
            local.get $var3
            local.get $var13
            i32.gt_s
            select
            i32.sub
            local.set $var7
            local.get $var3
            i32.const 2
            i32.shl
            local.set $var10
            i32.const 0
            local.set $var4
            local.get $var2
            i32.const 28
            i32.lt_u
            local.set $var14
            local.get $var6
            local.set $var2
            local.get $var3
            local.set $var5
            loop $label9
              block $label5
                block $label4
                  local.get $var4
                  local.get $var7
                  i32.add
                  i32.eqz
                  if
                    local.get $var6
                    i32.const 244
                    i32.add
                    local.set $var7
                    local.get $var8
                    i32.const 4
                    i32.shl
                    local.get $var6
                    i32.add
                    i32.const 4
                    i32.add
                    local.set $var8
                    i32.const 0
                    local.set $var2
                    br $label4
                  end
                  local.get $var5
                  i32.const 1
                  i32.sub
                  i32.const 59
                  i32.gt_u
                  br_if $label0
                  local.get $var2
                  local.get $var10
                  i32.add
                  local.tee $var17
                  i32.load
                  local.set $var1
                  local.get $var5
                  local.get $var3
                  local.get $var4
                  i32.add
                  local.get $var3
                  i32.div_u
                  local.tee $var15
                  local.get $var3
                  i32.mul
                  i32.sub
                  local.tee $var18
                  i32.eqz
                  if
                    local.get $var15
                    i32.const 1
                    i32.sub
                    local.tee $var15
                    i32.const 15
                    i32.gt_u
                    br_if $label0
                    local.get $var15
                    i32.const 91408
                    i32.add
                    i32.load8_u
                    i32.const 24
                    i32.shl
                    local.get $var1
                    i32.const 8
                    i32.rotl
                    call $func252
                    i32.xor
                    local.set $var1
                    br $label5
                  end
                  local.get $var14
                  local.get $var18
                  i32.const 4
                  i32.ne
                  i32.or
                  br_if $label5
                  local.get $var1
                  call $func252
                  local.set $var1
                  br $label5
                end $label4
                loop $label8
                  block $label6
                    local.get $var2
                    local.get $var13
                    i32.lt_s
                    if
                      i32.const 0
                      local.set $var4
                      local.get $var2
                      i32.const 0
                      i32.ne
                      local.get $var2
                      i32.const 4
                      i32.add
                      local.tee $var3
                      local.get $var13
                      i32.lt_s
                      i32.and
                      local.set $var14
                      local.get $var7
                      local.set $var10
                      local.get $var8
                      local.set $var1
                      loop $label7
                        local.get $var4
                        i32.const 4
                        i32.eq
                        br_if $label6
                        local.get $var4
                        local.get $var12
                        i32.add
                        i32.const 59
                        i32.gt_u
                        br_if $label0
                        local.get $var1
                        i32.load
                        local.set $var5
                        local.get $var14
                        if
                          local.get $var5
                          i32.const 255
                          i32.and
                          i32.const 91424
                          i32.add
                          i32.load8_u
                          i32.const 2
                          i32.shl
                          i32.const 99104
                          i32.add
                          i32.load
                          local.get $var5
                          i32.const 8
                          i32.shr_u
                          i32.const 255
                          i32.and
                          i32.const 91424
                          i32.add
                          i32.load8_u
                          i32.const 2
                          i32.shl
                          i32.const 98080
                          i32.add
                          i32.load
                          local.get $var5
                          i32.const 16
                          i32.shr_u
                          i32.const 255
                          i32.and
                          i32.const 91424
                          i32.add
                          i32.load8_u
                          i32.const 2
                          i32.shl
                          i32.const 97056
                          i32.add
                          i32.load
                          local.get $var5
                          i32.const 24
                          i32.shr_u
                          i32.const 91424
                          i32.add
                          i32.load8_u
                          i32.const 2
                          i32.shl
                          i32.const 96032
                          i32.add
                          i32.load
                          i32.xor
                          i32.xor
                          i32.xor
                          local.set $var5
                        end
                        local.get $var2
                        local.get $var4
                        i32.add
                        i32.const 59
                        i32.gt_u
                        br_if $label0
                        local.get $var10
                        local.get $var5
                        i32.store
                        local.get $var10
                        i32.const 4
                        i32.add
                        local.set $var10
                        local.get $var1
                        i32.const 4
                        i32.add
                        local.set $var1
                        local.get $var4
                        i32.const 1
                        i32.add
                        local.set $var4
                        br $label7
                      end $label7
                      unreachable
                    end
                    i32.const 0
                    local.set $var4
                    i32.const 0
                    local.set $var2
                    br $label3
                  end $label6
                  local.get $var7
                  i32.const 16
                  i32.add
                  local.set $var7
                  local.get $var12
                  i32.const 4
                  i32.sub
                  local.set $var12
                  local.get $var8
                  i32.const 16
                  i32.sub
                  local.set $var8
                  local.get $var3
                  local.set $var2
                  br $label8
                end $label8
                unreachable
              end $label5
              local.get $var5
              i32.const 60
              i32.eq
              local.get $var4
              i32.const 59
              i32.gt_u
              i32.or
              br_if $label0
              local.get $var17
              i32.const 4
              i32.add
              local.get $var2
              i32.const 4
              i32.add
              local.tee $var2
              i32.load
              local.get $var1
              i32.xor
              i32.store
              local.get $var4
              i32.const 1
              i32.add
              local.set $var4
              local.get $var5
              i32.const 1
              i32.add
              local.set $var5
              br $label9
            end $label9
            unreachable
          end
          local.get $var8
          local.get $var2
          local.get $var4
          i32.lt_u
          i32.or
          br_if $label0
          local.get $var4
          local.get $var6
          i32.add
          i32.const 4
          i32.add
          local.get $var4
          local.get $var7
          i32.add
          local.get $var1
          call $func202
          i32.store
          local.get $var5
          i32.const 1
          i32.sub
          local.set $var5
          local.get $var1
          i32.const 4
          i32.sub
          local.set $var1
          local.get $var4
          i32.const 4
          i32.add
          local.set $var4
          br $label10
        end $label10
        unreachable
      end $label0
      unreachable
    end $label3
    local.get $var11
    local.get $var4
    i32.store offset=4
    local.get $var11
    local.get $var6
    i32.store
    local.get $var11
    local.get $var2
    i32.store offset=8
    i32.const 177372
    local.get $var16
    i32.store
    local.get $var9
    i32.load offset=12
    local.set $var1
    local.get $var9
    i32.load offset=8
    local.set $var2
    local.get $var0
    local.get $var9
    i32.load offset=16
    i32.store offset=8
    local.get $var0
    local.get $var2
    i32.store
    local.get $var0
    local.get $var1
    i32.store offset=4
    local.get $var9
    i32.const 48
    i32.add
    global.set $global0
  )
