# umutkorkmaz0a

## Facebook Mail and Password
- https://tr.emailfake.com/dipet@682653.com and fb0000
<br>Same as https://www.facebook.com/umut.korkmaz.160/ have already decided.<br>
- https://tr.emailfake.com/empecheur@682653.com and fb0000
<br>Same as Adriana Ismailovic.<br>
- https://tr.emailfake.com/hanaha@682653.com and fb0000
<br>Same as https://www.facebook.com/people/Risa-Kaplan/34133/ have already decided.<br>
- https://tr.emailfake.com/indovinavi@682653.com and fb0000
<br>Same as Belkıs Yeter.
## Google Mail and Password
- dek00230@eoopy.com and gmail_00
- kvf84423@eoopy.com and gmail_00
## Tiktok Username
- umutumut720
- umutumut721
## Example code
```lua
do
	local seed = 6369051672525772
	math.randomseed = function (_seed)
		seed = math.floor(_seed) % 9007199254740992
	end
	math.random = function ()
		for a = 1, 53 do
			local carry = seed % 2 < 1
			seed = seed / 2
			seed = seed - seed % 1
			if carry then
				local z = 6369051672525773
				local x = 1
				for a = 1, 53 do
					local y = x * 2
					if z % y >= x then
						if seed % y < x then
							seed = seed + x
						else
							seed = seed - x
						end
					end
					x = y
				end
			end
		end
		return seed / 9007199254740992
	end
	table.shuffle = function (tbl)
		local n = #tbl
		for x = 1, n do
			local y = math.floor(math.random() * n + 1)
			local temp = tbl[x]
			tbl[x] = tbl[y]
			tbl[y] = temp
		end
	end
	table.sort = function (tbl, cmp)
		local n = #tbl
		for x = 1, n - 1 do
			for y = x + 1, n do
				local a
				if cmp ~= nil then
					a = cmp(tbl[y], tbl[x])
				else
					a = tbl[y] < tbl[x]
				end
				if a then
					local temp = tbl[x]
					tbl[x] = tbl[y]
					tbl[y] = temp
				end
			end
		end
	end
end
math.randomseed(os.time())
local a = {"22755", "25094", "5025", "6025", "28510", "32042", "34133", "23193"}
table.shuffle(a)
for x, y in ipairs(a) do print(x .. " = " .. y) end
```
