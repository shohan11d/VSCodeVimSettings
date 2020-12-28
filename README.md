# VSCodeVim Settings

VSCodeVim is a Vim emulator for Visual Studio Code + Commands

## Git Commands

### - Normal Mode

| Status             | Command          | Description                       |
| ------------------ | ---------------- | --------------------------------- |
| :white_check_mark: | `<leader>` gg    | Focus On Source Control View      |
| :white_check_mark: | `<leader>` gtl    | Focus On Timeline View            |
| :white_check_mark: | `<leader>` gir   | Git Initialize Repository         |
| :white_check_mark: | `<leader>` gai   | Git Add To .gitignore             |
| :white_check_mark: | `<leader>` gar   | Git Add Remote                    |
| :white_check_mark: | `<leader>` grr   | Git Remove Remote                 |
| :white_check_mark: | `<leader>` gsc   | Git Stage Change                  |
| :white_check_mark: | `<leader>` gsac  | Git Stage All Changes             |
| :white_check_mark: | `<leader>` gsamc | Git Stage All Merge Changes       |
| :white_check_mark: | `<leader>` gsatc | Git Stage All Tracked Changes     |
| :white_check_mark: | `<leader>` gsauc | Git Stage All Untracked Changes   |
| :white_check_mark: | `<leader>` guc   | Git Unstage Changes               |
| :white_check_mark: | `<leader>` guac  | Git Unstage All Changes           |
| :white_check_mark: | `<leader>` gcc   | Git Commit                        |
| :white_check_mark: | `<leader>` gca   | Git Commit All                    |
| :white_check_mark: | `<leader>` gcs   | Git Commit Staged                 |
| :white_check_mark: | `<leader>` gce   | Git Commit Empty                  |
| :white_check_mark: | `<leader>` gulc  | Git Undo Last Commit              |
| :white_check_mark: | `<leader>` gp    | Git Push                          |
| :white_check_mark: | `<leader>` gpf   | Git Push (Force)                  |
| :white_check_mark: | `<leader>` gpbt  | Git Push To...                    |
| :white_check_mark: | `<leader>` gpbtf | Git Push To... (Force)            |
| :white_check_mark: | `<leader>` gP    | Git Pull                          |
| :white_check_mark: | `<leader>` gPf   | Git Pull From...                  |
| :white_check_mark: | `<leader>` gPr   | Git Pull (Rebase)                 |
| :white_check_mark: | `<leader>` gAr   | Git Abort Rebase                  |
| :white_check_mark: | `<leader>` gcb   | Git Create Branch                 |
| :white_check_mark: | `<leader>` gcbf  | Git Create Branch From            |
| :white_check_mark: | `<leader>` gdb   | Git Delete Branch                 |
| :white_check_mark: | `<leader>` gmb   | Git Merge Branch                  |
| :white_check_mark: | `<leader>` gpb   | Git Publish Branch                |
| :white_check_mark: | `<leader>` grb   | Git Rename Branch                 |
| :white_check_mark: | `<leader>` gRb   | Git Rebase Branch                 |
| :white_check_mark: | `<leader>` gC    | Git Checkout To                   |
| :white_check_mark: | `<leader>` gCd   | Git Checkout To (Detached)        |
| :white_check_mark: | `<leader>` gcp   | Git Cherry Pick                   |
| :white_check_mark: | `<leader>` gdc   | Git Discard Changes               |
| :white_check_mark: | `<leader>` gdac  | Git Discard All Changes           |
| :white_check_mark: | `<leader>` gdatc | Git Discard All Tracked Changes   |
| :white_check_mark: | `<leader>` gdauc | Git Discard All Untracked Changes |
| :white_check_mark: | `<leader>` gss   | Git Stash                         |
| :white_check_mark: | `<leader>` gsiu  | Git Stash (Include Untracked)     |
| :white_check_mark: | `<leader>` gas   | Git Apply Stash                   |
| :white_check_mark: | `<leader>` gals  | Git Apply Latest Stash            |
| :white_check_mark: | `<leader>` gds   | Git Drop Stash                    |
| :white_check_mark: | `<leader>` gps   | Git Pop Stash                     |
| :white_check_mark: | `<leader>` gpls  | Git Pop Latest Stash              |
| :white_check_mark: | `<leader>` gct   | Git Create Tag                    |
| :white_check_mark: | `<leader>` gdt   | Git Delete Tag                    |
| :white_check_mark: | `<leader>` gpt   | Git Push Tags                     |
| :white_check_mark: | `<leader>` gff   | Git Fetch                         |
| :white_check_mark: | `<leader>` gfp   | Git Fetch (Prune)                 |
| :white_check_mark: | `<leader>` gffar | Git Fetch From All Remotes        |
| :white_check_mark: | `<leader>` goc   | Git Open Changes                  |
| :white_check_mark: | `<leader>` gof   | Git Open File                     |

<br>
<details>
 <summary><strong>Quick Example</strong> (click to expand)</summary>

Below is an example of a [settings.json](https://code.visualstudio.com/Docs/customization/userandworkspace) file with settings relevant to VSCodeVim:

```json
{
	"vim.normalModeKeyBindingsNonRecursive": [
		{
			"before": ["leader", "g", "g"],
			"commands": ["workbench.scm.focus"]
		},
		{
			"before": ["leader", "g", "t", "l"],
			"commands": ["timeline.focus"]
		},
		{
			"before": ["leader", "g", "i", "r"],
			"commands": ["git.init"]
		},
		{
			"before": ["leader", "g", "a", "i"],
			"commands": ["git.ignore"]
		},
		{
			"before": ["leader", "g", "a", "r"],
			"commands": ["git.addRemote"]
		},
		{
			"before": ["leader", "g", "r", "r"],
			"commands": ["git.removeRemote"]
		},
		{
			"before": ["leader", "g", "s", "c"],
			"commands": ["git.stage"]
		},
		{
			"before": ["leader", "g", "s", "a", "c"],
			"commands": ["git.stageAll"]
		},
		{
			"before": ["leader", "g", "s", "a", "m", "c"],
			"commands": ["git.stageAllMerge"]
		},
		{
			"before": ["leader", "g", "s", "a", "t", "c"],
			"commands": ["git.stageAllTracked"]
		},
		{
			"before": ["leader", "g", "s", "a", "t", "c"],
			"commands": ["git.stageAllUntracked"]
		},
		{
			"before": ["leader", "g", "u", "c"],
			"commands": ["git.unstage"]
		},
		{
			"before": ["leader", "g", "u", "a", "c"],
			"commands": ["git.unstageAll"]
		},
		{
			"before": ["leader", "g", "c", "c"],
			"commands": ["git.commit"]
		},
		{
			"before": ["leader", "g", "c", "a"],
			"commands": ["git.commitAll"]
		},
		{
			"before": ["leader", "g", "c", "s"],
			"commands": ["git.commitStaged"]
		},
		{
			"before": ["leader", "g", "c", "e"],
			"commands": ["git.commitEmpty"]
		},
		{
			"before": ["leader", "g", "u", "l", "c"],
			"commands": ["git.undoCommit"]
		},
		{
			"before": ["leader", "g", "p"],
			"commands": ["git.push"]
		},
		{
			"before": ["leader", "g", "p", "f"],
			"commands": ["git.pushForce"]
		},
		{
			"before": ["leader", "g", "p", "b", "t"],
			"commands": ["git.pushTo"]
		},
		{
			"before": ["leader", "g", "p", "b", "t", "f"],
			"commands": ["git.pushToForce"]
		},
		{
			"before": ["leader", "g", "P"],
			"commands": ["git.pull"]
		},
		{
			"before": ["leader", "g", "P", "f"],
			"commands": ["git.pullFrom"]
		},
		{
			"before": ["leader", "g", "P", "r"],
			"commands": ["git.pullRebase"]
		},
		{
			"before": ["leader", "g", "A", "r"],
			"commands": ["git.rebaseAbort"]
		},
		{
			"before": ["leader", "g", "c", "b"],
			"commands": ["git.branch"]
		},
		{
			"before": ["leader", "g", "c", "b", "f"],
			"commands": ["git.branchFrom"]
		},
		{
			"before": ["leader", "g", "d", "b"],
			"commands": ["git.deleteBranch"]
		},
		{
			"before": ["leader", "g", "m", "b"],
			"commands": ["git.merge"]
		},
		{
			"before": ["leader", "g", "p", "b"],
			"commands": ["git.publish"]
		},
		{
			"before": ["leader", "g", "r", "b"],
			"commands": ["git.renameBranch"]
		},
		{
			"before": ["leader", "g", "R", "b"],
			"commands": ["git.rebase"]
		},
		{
			"before": ["leader", "g", "C"],
			"commands": ["git.checkout"]
		},
		{
			"before": ["leader", "g", "C", "d"],
			"commands": ["git.checkoutDetached"]
		},
		{
			"before": ["leader", "g", "c", "p"],
			"commands": ["git.cherryPick"]
		},
		{
			"before": ["leader", "g", "d", "c"],
			"commands": ["git.clean"]
		},
		{
			"before": ["leader", "g", "d", "a", "c"],
			"commands": ["git.cleanAll"]
		},
		{
			"before": ["leader", "g", "d", "a", "t", "c"],
			"commands": ["git.cleanAllTracked"]
		},
		{
			"before": ["leader", "g", "d", "a", "u", "c"],
			"commands": ["git.cleanAllUntracked"]
		},
		{
			"before": ["leader", "g", "s", "s"],
			"commands": ["git.stash"]
		},
		{
			"before": ["leader", "g", "s", "i", "u"],
			"commands": ["git.stashIncludeUntracked"]
		},
		{
			"before": ["leader", "g", "a", "s"],
			"commands": ["git.stashApply"]
		},
		{
			"before": ["leader", "g", "a", "l", "s"],
			"commands": ["git.stashApplyLatest"]
		},
		{
			"before": ["leader", "g", "d", "s"],
			"commands": ["git.stashDrop"]
		},
		{
			"before": ["leader", "g", "p", "s"],
			"commands": ["git.stashPop"]
		},
		{
			"before": ["leader", "g", "p", "l", "s"],
			"commands": ["git.stashPopLatest"]
		},
		{
			"before": ["leader", "g", "c", "t"],
			"commands": ["git.createTag"]
		},
		{
			"before": ["leader", "g", "d", "t"],
			"commands": ["git.deleteTag"]
		},
		{
			"before": ["leader", "g", "p", "t"],
			"commands": ["git.pushTags"]
		},
		{
			"before": ["leader", "g", "f", "f"],
			"commands": ["git.fetch"]
		},
		{
			"before": ["leader", "g", "f", "p"],
			"commands": ["git.fetchPrune"]
		},
		{
			"before": ["leader", "g", "f", "f", "a", "r"],
			"commands": ["git.fetchAll"]
		},
		{
			"before": ["leader", "g", "o", "c"],
			"commands": ["git.openChange"]
		},
		{
			"before": ["leader", "g", "o", "f"],
			"commands": ["git.openFile"]
		}
	]
}
```

</details>
<br>
<br>

### - Visual Mode

in visual mode

| Status             | Command       | Description                 |
| ------------------ | ------------- | --------------------------- |
| :white_check_mark: | `<leader>` gs | Git Stage Selected Ranges   |
| :white_check_mark: | `<leader>` gu | Git Unstage Selected Ranges |
| :white_check_mark: | `<leader>` gr | Git Revert Selected Ranges  |

<br>
<details>
 <summary><strong>Quick Example</strong> (click to expand)</summary>

Below is an example of a [settings.json](https://code.visualstudio.com/Docs/customization/userandworkspace) file with settings relevant to VSCodeVim:

```json
{
	"vim.visualModeKeyBindingsNonRecursive": [
		{
			"before": ["<Leader>", "g", "s"],
			"commands": ["git.stageSelectedRanges"]
		},
		{
			"before": ["<Leader>", "g", "u"],
			"commands": ["git.unstageSelectedRanges"]
		},
		{
			"before": ["<Leader>", "g", "r"],
			"commands": ["git.revertSelectedRanges"]
		}
	]
}
```

</details>
<br>
<br>

## Emmet Commands

### - Normal Mode

| Status             | Command        | Description                     |
| ------------------ | -------------- | ------------------------------- |
| :white_check_mark: | `<leader>` ei0 | Emmet Increment by 0.1          |
| :white_check_mark: | `<leader>` ed0 | Emmet Decrement by 0.1          |
| :white_check_mark: | `<leader>` eiu | Emmet Increment by 1            |
| :white_check_mark: | `<leader>` edu | Emmet Decrement by 1            |
| :white_check_mark: | `<leader>` eid | Emmet Increment by 10           |
| :white_check_mark: | `<leader>` edd | Emmet Decrement by 10           |
| :white_check_mark: | `<leader>` et  | Emmet Go To Matching Pair       |
| :white_check_mark: | `<leader>` enp | Emmet Go To Next Edit Point     |
| :white_check_mark: | `<leader>` epp | Emmet Go To Previous Edit Point |
| :white_check_mark: | `<leader>` ex  | Emmet Evaluate Math Expression  |
| :white_check_mark: | `<leader>` eml | Emmet Merge Lines               |
| :white_check_mark: | `<leader>` eut | Emmet Update Tag                |
| :white_check_mark: | `<leader>` ert | Emmet Remove Tag                |
| :white_check_mark: | `<leader>` esj | Emmet Split / Join Tag          |
| :white_check_mark: | `<leader>` eui | Emmet Update Image Size         |
| :white_check_mark: | `<leader>` ec  | Emmet Toggle Comment            |
| :white_check_mark: | `<leader>` erc | Emmet Reflect CSS Value         |
| :white_check_mark: | `<leader>` ew  | Emmet Wrap with Abbreviation    |

<br>
<details>
 <summary><strong>Quick Example</strong> (click to expand)</summary>

Below is an example of a [settings.json](https://code.visualstudio.com/Docs/customization/userandworkspace) file with settings relevant to VSCodeVim:

```json
{
	"vim.normalModeKeyBindingsNonRecursive": [
		{
			"before": ["<Leader>", "e", "b", "i"],
			"commands": ["editor.emmet.action.balanceIn"]
		},
		{
			"before": ["<Leader>", "e", "b", "o"],
			"commands": ["editor.emmet.action.balanceOut"]
		},
		{
			"before": ["<Leader>", "e", "i", "0"],
			"commands": ["editor.emmet.action.incrementNumberByOneTenth"]
		},
		{
			"before": ["<Leader>", "e", "d", "0"],
			"commands": ["editor.emmet.action.decrementNumberByOneTenth"]
		},
		{
			"before": ["<Leader>", "e", "i", "u"],
			"commands": ["editor.emmet.action.incrementNumberByOne"]
		},
		{
			"before": ["<Leader>", "e", "d", "u"],
			"commands": ["editor.emmet.action.decrementNumberByOne"]
		},
		{
			"before": ["<Leader>", "e", "i", "d"],
			"commands": ["editor.emmet.action.incrementNumberByTen"]
		},
		{
			"before": ["<Leader>", "e", "d", "d"],
			"commands": ["editor.emmet.action.decrementNumberByTen"]
		},
		{
			"before": ["<Leader>", "e", "t"],
			"commands": ["editor.emmet.action.matchTag"]
		},
		{
			"before": ["<Leader>", "e", "n"],
			"commands": ["editor.emmet.action.nextEditPoint"]
		},
		{
			"before": ["<Leader>", "e", "p"],
			"commands": ["editor.emmet.action.prevEditPoint"]
		},
		{
			"before": ["<Leader>", "e", "x"],
			"commands": ["editor.emmet.action.evaluateMathExpression"]
		},
		{
			"before": ["<Leader>", "e", "m", "l"],
			"commands": ["editor.emmet.action.mergeLines"]
		},
		{
			"before": ["<Leader>", "e", "u", "t"],
			"commands": ["editor.emmet.action.updateTag"]
		},
		{
			"before": ["<Leader>", "e", "r", "t"],
			"commands": ["editor.emmet.action.removeTag"]
		},
		{
			"before": ["<Leader>", "e", "s", "j"],
			"commands": ["editor.emmet.action.splitJoinTag"]
		},
		{
			"before": ["<Leader>", "e", "u", "i"],
			"commands": ["editor.emmet.action.updateImageSize"]
		},
		{
			"before": ["<Leader>", "e", "c"],
			"commands": ["editor.emmet.action.toggleComment"]
		},
		{
			"before": ["<Leader>", "e", "r", "c"],
			"commands": ["editor.emmet.action.reflectCSSValue"]
		},
		{
			"before": ["<Leader>", "e", "w"],
			"commands": ["editor.emmet.action.wrapWithAbbreviation"]
		}
	]
}
```

</details>
<br>
<br>

### - Visual Mode

in visual mode

| Status             | Command        | Description                                   |
| ------------------ | -------------- | --------------------------------------------- |
| :white_check_mark: | `<leader>` ebi | Emmet Balance (inward)                        |
| :white_check_mark: | `<leader>` ebo | Emmet Balance (outward)                       |
| :white_check_mark: | `<leader>` et  | Emmet Go To Matching Pair                     |
| :white_check_mark: | `<leader>` ec  | Emmet Toggle Comment                          |
| :white_check_mark: | `<leader>` en  | Emmet Select Next Item                        |
| :white_check_mark: | `<leader>` ep  | Emmet Select Previous Item                    |
| :white_check_mark: | `<leader>` ex  | Emmet Evaluate Math Expression                |
| :white_check_mark: | `<leader>` ew  | Emmet Wrap Individual Lines with Abbreviation |

<br>
<details>
 <summary><strong>Quick Example</strong> (click to expand)</summary>

Below is an example of a [settings.json](https://code.visualstudio.com/Docs/customization/userandworkspace) file with settings relevant to VSCodeVim:

```json
{
	"vim.visualModeKeyBindingsNonRecursive": [
		{
			"before": ["<Leader>", "e", "b", "i"],
			"commands": ["editor.emmet.action.balanceIn"]
		},
		{
			"before": ["<Leader>", "e", "b", "o"],
			"commands": ["editor.emmet.action.balanceOut"]
		},
		{
			"before": ["<Leader>", "e", "t"],
			"commands": ["editor.emmet.action.matchTag"]
		},
		{
			"before": ["<Leader>", "e", "c"],
			"commands": ["editor.emmet.action.toggleComment"]
		},
		{
			"before": ["<Leader>", "e", "n"],
			"commands": ["editor.emmet.action.selectNextItem"]
		},
		{
			"before": ["<Leader>", "e", "p"],
			"commands": ["editor.emmet.action.selectPrevItem"]
		},
		{
			"before": ["<Leader>", "e", "x"],
			"commands": ["editor.emmet.action.evaluateMathExpression"]
		},
		{
			"before": ["<Leader>", "e", "w"],
			"commands": [
				"editor.emmet.action.wrapIndividualLinesWithAbbreviation"
			]
		}
	]
}
```

</details>
<br>
<br>
