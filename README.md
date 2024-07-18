THIS IS FORKED SYNSAVEINSTANCE THINGY BUT ME MIXZ CUSTOMIZED IT
# Loadstring

```lua
-- modified by @Mixzondc

local Params = {
    RepoURL = "https://raw.githubusercontent.com/luau/SynSaveInstance/main/",
    SSI = "saveinstance",
}

local synsaveinstance = loadstring(game:HttpGet(Params.RepoURL .. Params.SSI .. ".luau", true), Params.SSI)()

local CustomOptions = {
    mode = "custom",
    ExtraInstances = {game.workspace, game.ReplicatedStorage, game.Lighting, game.ReplicatedFirst, game.StarterPack, game.Lighting, game.Players, game.StarterPlayer, game.StarterGui},
    --ExtraInstances = {game.workspace, game.Lighting},
    Decompile = true,
    decomptype = "custom", -- remove this line if you using wave.
    noscripts = false,
    Anonymous = true,
    TreatUnionsAsParts = true,
    RemovePlayerCharacters = false,
    IsolateLocalPlayerCharacter = true,
}

synsaveinstance(CustomOptions)
```


