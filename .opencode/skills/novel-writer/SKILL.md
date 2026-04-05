---
name: novel-writer
description: |
  Generates chapters for the novel "量化神明：代碼與信仰的套利交易" following standardized SOP
  
  Triggers when user mentions:
  - "generate chapter" or "write chapter [N]"
  - "continue the novel" or "next chapter"
  - "novel SOP" or "chapter template"
  - "生成第N章"
---

## Quick Usage (Already Configured)

### Generate Next Chapter
```bash
# Follow the complete SOP workflow below
```

---

## 一、 Standardized Workflow (SOP)

### Pre-Generation Checklist

#### 1.1 File Locations
| Type | Path | Example |
|------|------|---------|
| Chapter | `chapters/ch{NN}.md` | `chapters/ch21.md` |
| Spec | `.sisyphus/plans/novel-spec.md` | - |
| SOP | `.sisyphus/plans/novel-sop.md` | - |
| Structure | `.sisyphus/plans/novel-structure-chX-Y.md` | `novel-structure-ch21-30.md` |
| Execution | `.sisyphus/plans/novel-writing-chX-Y.md` | `novel-writing-ch21-30.md` |

#### 1.2 Pre-Generation Checklist
- [ ] Read previous chapter's ending global memo
- [ ] Confirm current asset status
- [ ] Confirm current suspense/plot threads
- [ ] Confirm character statuses
- [ ] Check novel-spec.md is latest version
- [ ] Confirm writing proportions (5% tech + 30% scene + 35% psychology + 30% dialogue)
- [ ] Reference structure plan for this chapter's plot

### Generation Workflow (5 Steps)

#### Step 1: Read Previous Chapter's Global Memo
- Confirm current timeline
- Confirm asset status
- Confirm suspense and plot threads
- Confirm character statuses

#### Step 2: Check and Update Spec File
- Confirm spec version is latest (novel-spec.md)
- Confirm tech ratio is 5%
- Confirm asset data is accurate

#### Step 3: Create Chapter Outline Plan (if needed)
- If new volume (every 10 chapters), create detailed outline
- Define core plot for each chapter
- Define suspense arrangement

#### Step 4: Generate Single Chapter
Follow template proportions:
- **Tech atmosphere (5%)**: ~100 words - one sentence passing through tech element
- **Scene/Sensory (30%)**: ~600 words - environment, atmosphere, sensory details
- **Psychology (35%)**: ~700 words - character's inner struggle, PM thinking, quant thinking
- **Dialogue/Action (30%)**: ~600 words - dialogue clashes, expressions, actions

Template:
```markdown
# 第 N 章：[標題]

[第一段：場景描寫 + 與上一章懸念銜接]
- 描述當前場景
- 銜接上一章的結尾

[主體段落：按比例分配]
- 技術氛圍（一句話）
- 場景描寫
- 心理獨白
- 對話與動作

[結尾段落：懸念]
- 為下一章做鋪墊

---
> **全局記憶備忘錄更新：**
> * 當前時間線：Day N — [時間段]
> * 主角資產狀態：[BTC、功德等]
> * 重要伏筆與未解之謎：
>   - 懸念1
>   - 懸念2
> * 登場人物/神明狀態：[狀態]
```

#### Step 5: Verify and Commit
- [ ] Check asset changes are reasonable
- [ ] Check suspense continues
- [ ] Check word count ~2000
- [ ] Check tech ratio is 5%
- [ ] Git commit and push

---

## 二、 Writing Proportions

| Element | Percentage | Words Reference |
|---------|------------|------------------|
| Tech atmosphere | 5% | ~100 words (one sentence pass) |
| Scene/Sensory | 30% | ~600 words |
| Psychology | 35% | ~700 words |
| Dialogue/Action | 30% | ~600 words |
| **Total** | 100% | **~2000 words** |

---

## 三、 Global Memo Format (Required at End of Each Chapter)

```markdown
---
> **全局記憶備忘錄更新：**
> * 當前時間線：Day N — [時間段]
> * 主角資產狀態：[BTC、功德等]
> * 重要伏筆與未解之謎：
>   - [懸念1]
>   - [懸念2]
> * 登場人物/神明狀態：[狀態]
```

---

## 四、 Current Progress Tracking

### Completed Chapters
- ✅ Ch.1-10 (第一卷)
- ✅ Ch.11-20 (第二卷)
- ⏳ Ch.21-30 (第三卷 - in progress)

### Current Asset Status (Ch.20 Ending)
- BTC: 1.87
- 功德 Token: 684,931
- 因果信用評分: 770
- 因果律偏差值: 0.912
- 最終防禦系統: 啟動中（24小時倒數）

---

## 五、 Git Commit Standard

### Commit Message Format
```
[類型]: [簡短描述]

- 詳細內容1
- 詳細內容2
- 詳細內容3

Ultraworked with [Sisyphus]
Co-authored-by: Sisyphus <clio-agent@sisyphuslabs.ai>
```

### Commit Types
- `feat`: 新情節/new plot
- `fix`: 修復/fix
- `docs`: 文檔更新/docs
- `chore`: 其他更新/chore
