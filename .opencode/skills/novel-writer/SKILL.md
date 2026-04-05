---
name: novel-writer
description: |
  Generates chapters for the novel "量化神明：代碼與信仰的套利交易" following standardized SOP
  
  Triggers when user mentions:
  - "generate chapter" or "write chapter"
  - "continue the novel" or "next chapter"
  - "novel SOP" or "chapter template"
---

## Quick Usage (Already Configured)

### Generate Next Chapter
```bash
# 1. Read previous chapter's ending memo
# 2. Check novel-spec.md for latest specifications
# 3. Generate chapter following SOP template
# 4. Commit and push
```

### File Locations
- Chapters: `chapters/ch{NN}.md`
- Spec: `.sisyphus/plans/novel-spec.md`
- SOP: `.sisyphus/plans/novel-sop.md`
- Structure: `.sisyphus/plans/novel-structure-chX-Y.md`
- Execution: `.sisyphus/plans/novel-writing-chX-Y.md`

### Workflow
```
1. Read previous chapter's global memo
2. Check spec version
3. Generate chapter (~2000 words)
4. Update global memo
5. Git commit + push
```

## Writing Proportions

| Element | Percentage | Words |
|---------|------------|-------|
| Tech atmosphere | 5% | ~100 |
| Scene/Sensory | 30% | ~600 |
| Psychology | 35% | ~700 |
| Dialogue/Action | 30% | ~600 |

## Global Memo Format

```markdown
---
> **全局記憶備忘錄更新：**
> * 當前時間線：Day N — [時間段]
> * 主角資產狀態：[BTC、功德等]
> * 重要伏筆與未解之謎：
>   - 懸念1
>   - 懸念2
> * 登場人物/神明狀態：[狀態]
```
