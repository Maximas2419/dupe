local n = 120000
for i = 1, n do
print("Succesfully executed once")
workspace.__THINGS.__REMOTES.MAIN:FireServer("b", "bank withdraw")
local function Bank(id)
  local self = {}
  function self:withdraw(pets, gems)
local A_1 =
{
   [1] = id,
   [2] =
{
},
   [3] = gems
}
       local Event = game:GetService("Workspace")["__THINGS"]["__REMOTES"]["bank withdraw"]
       Event:InvokeServer(A_1)
  end
  return self
end
--//
local bankid = "26933480-9c8d-4110-a068-4a9306c516aa"--bank
for i=1, 1 do
  Bank(bankid):withdraw({}, 1)
  print('withdrawed 1 gem')
  task.wait()
end
wait(2.0)
end
