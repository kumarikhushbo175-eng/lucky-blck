# Quick Start Guide - After Downloading ZIP

## 📥 Steps After Downloading lucky-blck.zip

### **Step 1: Extract the ZIP File**
```
1. Right-click lucky-blck.zip
2. Select "Extract All..." (Windows) or "Extract" (Mac)
3. Choose a folder location
4. Wait for extraction to complete
```

**You should now see:**
```
lucky-blck/
├── behavior_pack/
├── resource_pack/
├── docs/
├── README.md
├── LICENSE
└── CHANGELOG.md
```

---

### **Step 2: Find Your Minecraft Folder**

**Windows 10/11:**
1. Press `Windows Key + R`
2. Type: `%APPDATA%`
3. Navigate to: `Roaming\Microsoft\Windows\Start Menu\Programs\Minecraft\`
4. Look for **"Minecraft Launcher"**
5. OR Go to: `C:\Users\[YOUR_USERNAME]\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\`

**Easier Method - Use File Explorer:**
```
C:\Users\[YOUR_USERNAME]\AppData\Local\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\
```

---

### **Step 3: Copy Packs to Minecraft Folder**

**Inside the Minecraft folder you found, locate:**
```
com.mojang/
└── development_packs/
```

**If "development_packs" doesn't exist, create it:**
1. Right-click in the com.mojang folder
2. New → Folder
3. Name it: `development_packs`

---

### **Step 4: Copy Your Packs**

**From your extracted lucky-blck folder:**

1. Copy the entire **behavior_pack** folder
   - Paste it into: `development_packs/`
   
2. Copy the entire **resource_pack** folder
   - Paste it into: `development_packs/`

**Result should be:**
```
development_packs/
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

---

### **Step 5: Open Minecraft Bedrock**

1. Open **Minecraft Bedrock Edition**
2. Click **"Create New World"**
3. Set your world name and settings

---

### **Step 6: Add Packs to Your World**

**This is CRITICAL - Follow order exactly:**

#### **First - Add Resource Pack:**
1. Click **"Resource Packs"** button
2. Click **"My Packs"** tab
3. You should see **"Lucky Block Resources"**
4. Click it to select it
5. Click **"Activate"** button
6. It will move to "Active" section

#### **Second - Add Behavior Pack:**
1. Click **"Behavior Packs"** button
2. Click **"My Packs"** tab
3. You should see **"Lucky Block Behaviors"**
4. Click it to select it
5. Click **"Activate"** button
6. It will move to "Active" section

**IMPORTANT:** Resource pack MUST be above behavior pack in the list!

---

### **Step 7: Create World**

1. Click **"Create"** button at bottom right
2. Wait for world to load
3. You're in the world!

---

### **Step 8: Test the Lucky Block**

**In Creative Mode:**
1. Press `T` to open chat
2. Type: `/give @s lucky:lucky_block`
3. Press Enter
4. You should get a Lucky Block in your inventory

**Break the block:**
1. Place it on the ground
2. Break it with any tool
3. Random items should drop!

**If it works:** 🎉 You're all set!

---

### **🐛 Troubleshooting - What if Packs Don't Show Up?**

**Issue: "Lucky Block Resources" not found**

**Solution:**
1. Restart Minecraft completely
2. Close the launcher
3. Reopen Minecraft
4. Try again

**If still not working:**
1. Check if development_packs folder exists
2. Verify folder names have NO spaces
3. Restart Windows
4. Try copying packs again

---

### **🐛 Troubleshooting - "Failed to Import" Error**

**If you get "Failed to Import" when trying to activate:**

1. Delete both packs from development_packs
2. Restart Minecraft
3. Copy packs again (fresh copy)
4. Try importing again

**If still failing:**
1. Check manifest.json files are valid
2. Make sure PNG files exist in resource_pack/textures/blocks/
3. Check folder names match exactly

---

### **🐛 Troubleshooting - Block is Invisible/Pink**

**If Lucky Block appears pink or invisible:**

1. Make sure resource pack is enabled FIRST
2. Check PNG files in: `resource_pack/textures/blocks/`
3. Files needed:
   - lucky_block_top.png
   - lucky_block_side.png
   - lucky_block_bottom.png
4. Restart resource pack

---

### **✅ Complete Checklist**

- [ ] Extracted ZIP file
- [ ] Found Minecraft folder
- [ ] Created development_packs folder
- [ ] Copied behavior_pack to development_packs
- [ ] Copied resource_pack to development_packs
- [ ] Opened Minecraft
- [ ] Activated resource pack FIRST
- [ ] Activated behavior pack SECOND
- [ ] Created new world with both packs
- [ ] Tested with `/give @s lucky:lucky_block`
- [ ] Block drops items when broken ✅

---

### **📝 Useful Commands**

```
/give @s lucky:lucky_block           # Get Lucky Block
/clear @s                             # Clear inventory
/gamemode creative                    # Creative mode
/gamemode survival                    # Survival mode
/time set day                         # Set to daytime
/weather clear                        # Clear weather
```

---

### **🆘 Still Having Issues?**

1. **Check:** https://github.com/kumarikhushbo175-eng/lucky-blck/blob/main/docs/BEDROCK_PC_FIXES.md
2. **Read:** Installation troubleshooting section
3. **Verify:** All files are in correct locations
4. **Restart:** Minecraft completely

---

## 🎮 You're Ready to Play!

Your Lucky Block Mod is now installed and ready to use! 🎉

Enjoy the random rewards and have fun! ✨
