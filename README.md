function spawnPet(petName, x, y, z)
    -- Criação de uma nova instância do pet
    local pet = Instance.new("Part")
    pet.Name = petName or "MeuPet"
    pet.Position = Vector3.new(x or 0, y or 5, z or 0)
    pet.Size = Vector3.new(2, 2, 2)
    pet.BrickColor = BrickColor.new("Bright green")
    pet.Anchored = false

    -- Adiciona o pet ao workspace
    pet.Parent = workspace

    print("Pet spawnado: " .. pet.Name .. " em (" .. pet.Position.X .. ", " .. pet.Position.Y .. ", " .. pet.Position.Z .. ")")
end

-- Exemplo de uso:
spawnPet("PetDoAgas", 10, 5, 10)
