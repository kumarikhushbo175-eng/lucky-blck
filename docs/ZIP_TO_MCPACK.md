# How to Convert ZIP to MCPACK

## 📦 What is MCPACK?

MCPACK (Minecraft Pack) is a special format that allows one-click installation in Minecraft Bedrock Edition.

**Advantages:**
- ✅ One-click install in Minecraft
- ✅ Automatic file placement
- ✅ No manual folder copying needed
- ✅ Easier for sharing
- ✅ Prevents installation errors

---

## 🔧 Method 1: Manual Conversion (Windows)

### **Step 1: Prepare Files**

```
lucky-blck-final/
├── behavior_pack/
│   ├── manifest.json
│   ├── blocks/
│   ├── entities/
│   ├── loot_tables/
│   └── functions/
└── resource_pack/
    ├── manifest.json
    ├── textures/
    └── sounds.json
```

### **Step 2: Create Separate MCPACK Files**

**For Behavior Pack:**
1. Open behavior_pack folder
2. Select all files inside (NOT the folder itself)
3. Right-click → Send to → Compressed (zipped) folder
4. Rename to: `LuckyBlock_Behavior.zip`
5. Rename to: `LuckyBlock_Behavior.mcpack`

**For Resource Pack:**
1. Open resource_pack folder
2. Select all files inside (NOT the folder itself)
3. Right-click → Send to → Compressed (zipped) folder
4. Rename to: `LuckyBlock_Resource.zip`
5. Rename to: `LuckyBlock_Resource.mcpack`

---

## 🔧 Method 2: Using 7-Zip (Recommended)

### **Step 1: Install 7-Zip**
- Download: https://www.7-zip.org/
- Install it

### **Step 2: Create Behavior Pack MCPACK**
```
1. Right-click behavior_pack folder
2. 7-Zip → Add to archive
3. Name: LuckyBlock_Behavior.zip
4. Archive format: zip
5. Click OK
6. Rename file to: LuckyBlock_Behavior.mcpack
```

### **Step 3: Create Resource Pack MCPACK**
```
1. Right-click resource_pack folder
2. 7-Zip → Add to archive
3. Name: LuckyBlock_Resource.zip
4. Archive format: zip
5. Click OK
6. Rename file to: LuckyBlock_Resource.mcpack
```

---

## 🔧 Method 3: Using PowerShell (Advanced)

Open PowerShell as Administrator and run:

```powershell
# For Behavior Pack
Compress-Archive -Path "C:\path\to\behavior_pack\*" -DestinationPath "LuckyBlock_Behavior.zip"
Rename-Item "LuckyBlock_Behavior.zip" "LuckyBlock_Behavior.mcpack"

# For Resource Pack
Compress-Archive -Path "C:\path\to\resource_pack\*" -DestinationPath "LuckyBlock_Resource.zip"
Rename-Item "LuckyBlock_Resource.zip" "LuckyBlock_Resource.mcpack"
```

---

## ✅ Installing MCPACK Files

### **Method 1: Direct Click (Easiest)**
1. Double-click `LuckyBlock_Behavior.mcpack`
2. Minecraft should open
3. Click "Import" when prompted
4. Click "Activate" when asked

Repeat for `LuckyBlock_Resource.mcpack`

### **Method 2: Manual File Copy**
1. Copy `.mcpack` files
2. Navigate to: `C:\Users\[YOUR_USERNAME]\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\minecraftWorlds\[WORLD_NAME]\behavior_packs\`
3. Paste files there
4. Do same for resource_packs folder

### **Method 3: Through Minecraft UI**
1. Open Minecraft
2. Settings → Global Resources
3. Click folder icon
4. Copy `.mcpack` files into the opened folder
5. Restart Minecraft

---

## 📋 MCPACK File Checklist

**Before creating MCPACK, verify:**

- [ ] manifest.json is valid (not corrupted)
- [ ] All folder structure is correct
- [ ] PNG files exist and are 16x16
- [ ] No spaces in folder names
- [ ] JSON files are properly formatted
- [ ] UUID values are present in manifests

---

## 🎮 Testing MCPACK Installation

1. Create new Minecraft world
2. Double-click `.mcpack` file
3. Click "Import" in Minecraft prompt
4. Select resource pack first
5. Select behavior pack second
6. Create world
7. Test: `/give @s lucky:lucky_block`

---

## 📦 Download Ready MCPACK Files

If you want pre-made MCPACK files, you can:

1. Visit: https://github.com/kumarikhushbo175-eng/lucky-blck/releases
2. Download MCPACK versions
3. Double-click to install
4. Done! 🎉

---

## 🚀 Distribute Your MCPACK

Share MCPACK files on:
- **CurseForge**: https://www.curseforge.com/minecraft/
- **Planet Minecraft**: https://www.planetminecraft.com/
- **GitHub Releases**: Add to your repository
- **Discord**: Share in Minecraft modding servers

---

## 📝 Common Issues

### **Issue: MCPACK won't open**
- Solution: Right-click → Open with → Minecraft
- OR: Copy to com.mojang folder manually

### **Issue: File association broken**
- Solution: Right-click MCPACK → Properties → Change → Minecraft

### **Issue: Import fails**
- Solution: Check manifest.json is valid JSON
- Try: Delete and recreate MCPACK file

---

## ✅ Done!

Your Lucky Block Mod now has MCPACK files for easy distribution! 🎉

Users can now install with one click! 🚀
