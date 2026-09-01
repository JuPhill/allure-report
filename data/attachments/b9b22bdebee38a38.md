# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: 09_CustomerCustomFieldsTests.spec.js >> Customer Custom Fields Tests >> Move C3 field up, then rename C2 to "rename C2 to C3" and save
- Location: tests/09_CustomerCustomFieldsTests.spec.js:118:2

# Error details

```
Error: Clicking the label for 'C2' did not open an inline editor.
```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
  - navigation [ref=e2]:
    - generic [ref=e3]:
      - link "Skynamo" [ref=e5] [cursor=pointer]:
        - /url: /
        - img "Skynamo" [ref=e6]
      - generic [ref=e7]:
        - list [ref=e8]:
          - listitem [ref=e9]:
            - link "Timeline" [ref=e10] [cursor=pointer]:
              - /url: /Reports
          - listitem [ref=e11]:
            - link "Calendar" [ref=e12] [cursor=pointer]:
              - /url: /Reports/CalendarReports
          - listitem [ref=e13]:
            - link "Products" [ref=e14] [cursor=pointer]:
              - /url: /Products
          - listitem [ref=e15]:
            - link "Customers" [ref=e16] [cursor=pointer]:
              - /url: /Customers
          - listitem [ref=e17]:
            - link "Contacts" [ref=e18] [cursor=pointer]:
              - /url: /Contacts
          - listitem [ref=e19]:
            - link "Forms" [ref=e20] [cursor=pointer]:
              - /url: /Forms
          - listitem [ref=e21]:
            - link "Users" [ref=e22] [cursor=pointer]:
              - /url: /Users/Users
          - listitem [ref=e23]:
            - link "Reports" [ref=e24] [cursor=pointer]:
              - /url: /Reports/Reports/Index/0
        - list [ref=e25]:
          - listitem "Settings" [ref=e26]:
            - link [ref=e27] [cursor=pointer]:
              - /url: /MobileDevices
              - generic [ref=e28]: settings
          - listitem
          - listitem [ref=e29]:
            - link "phillip stg1" [ref=e30] [cursor=pointer]:
              - /url: "#menuUser"
              - text: phillip stg1
  - generic [ref=e33]:
    - button "Reset" [ref=e35] [cursor=pointer]
    - button "Save" [ref=e37] [cursor=pointer]
  - generic [ref=e39]:
    - generic [ref=e42]:
      - heading "Add a field" [level=4] [ref=e44]
      - generic [ref=e46]:
        - paragraph [ref=e47]: Click to add one of the following field types (Maximum of 240)
        - generic [ref=e48]:
          - button "Text" [ref=e49] [cursor=pointer]
          - button "Number" [ref=e50] [cursor=pointer]
          - button "Drop down box" [ref=e52] [cursor=pointer]: Drop down box
          - button "Email" [ref=e54] [cursor=pointer]
          - button "Address" [ref=e55] [cursor=pointer]
          - button "Date/Time" [ref=e56] [cursor=pointer]
          - button "Label" [ref=e57] [cursor=pointer]
          - button "Divider" [ref=e58] [cursor=pointer]
    - generic [ref=e61]:
      - heading "Customer fields" [level=4] [ref=e63]
      - generic [ref=e65]:
        - generic [ref=e68]: Label
        - generic [ref=e70]:
          - heading "C1" [level=5] [ref=e71]
          - combobox [ref=e72]:
            - option "Option 1" [selected]
            - option "Option 2"
            - option "Option 3"
        - heading "C3" [level=5] [ref=e75]
        - generic [ref=e76]:
          - generic [ref=e77]:
            - heading "Drop down box Multi select" [level=4] [ref=e78]
            - generic [ref=e79]:
              - generic "Delete" [ref=e80] [cursor=pointer]: delete
              - generic "Duplicate" [ref=e81] [cursor=pointer]: content_copy
              - generic "Move down" [ref=e82] [cursor=pointer]: arrow_downward
              - generic "Move up" [ref=e83] [cursor=pointer]: arrow_upward
          - generic [ref=e84]:
            - heading "C2" [level=5] [ref=e85]
            - combobox [ref=e86]:
              - option "Option 1" [selected]
              - option "Option 2"
              - option "Option 3"
        - heading "C4" [level=5] [ref=e89]
        - separator [ref=e92]
        - generic [ref=e94]:
          - heading "Number no decimals" [level=5] [ref=e95]
          - textbox [disabled] [ref=e96]: "0"
        - generic [ref=e98]:
          - heading "Number 2 decimals" [level=5] [ref=e99]
          - textbox [disabled] [ref=e100]: "0"
        - generic [ref=e102]:
          - heading "Drop Down Box Single Select" [level=5] [ref=e103]
          - combobox [ref=e104]:
            - option "Option 1" [selected]
            - option "Option 2"
            - option "Option 3"
        - generic [ref=e106]:
          - heading "Drop Down Box Multi Select" [level=5] [ref=e107]
          - combobox [ref=e108]:
            - option "Option 1" [selected]
            - option "Option 2"
            - option "Option 3"
        - heading "Drop Down Box Nested Single Select" [level=5] [ref=e111]
        - heading "Drop Down Box Nested Multi Select" [level=5] [ref=e114]
        - generic [ref=e116]:
          - heading "EMail do not send" [level=5] [ref=e117]
          - textbox [disabled] [ref=e118]: example@site.com
        - generic [ref=e120]:
          - heading "EMail send" [level=5] [ref=e121]
          - textbox [disabled] [ref=e122]: example@site.com
        - generic [ref=e124]:
          - heading "Address" [level=5] [ref=e125]
          - table [ref=e127]:
            - rowgroup [ref=e128]:
              - row "Street" [ref=e129]:
                - cell "Street" [ref=e130]:
                  - textbox [disabled] [ref=e131]: Street
              - row "Suburb" [ref=e132]:
                - cell "Suburb" [ref=e133]:
                  - textbox [disabled] [ref=e134]: Suburb
              - row "Town/City" [ref=e135]:
                - cell "Town/City" [ref=e136]:
                  - textbox [disabled] [ref=e137]: Town/City
              - row "Code" [ref=e138]:
                - cell "Code" [ref=e139]:
                  - textbox [disabled] [ref=e140]: Code
        - generic [ref=e142]:
          - heading "DD/MM/YYYY" [level=5] [ref=e143]
          - paragraph [ref=e144]: DD/MM/YYYY
        - generic [ref=e146]:
          - heading "DD/MM/YYYY HH:MM:SS" [level=5] [ref=e147]
          - paragraph [ref=e148]: DD/MM/YYYY HH:MM:SS
        - generic [ref=e150]:
          - heading "HH:MM" [level=5] [ref=e151]
          - paragraph [ref=e152]: HH:MM
        - generic [ref=e154]:
          - heading "HH:MM:SS" [level=5] [ref=e155]
          - paragraph [ref=e156]: HH:MM:SS
        - heading "Drop down box Nested single select11" [level=5] [ref=e159]
        - heading "Drop down box Nested multi select22" [level=5] [ref=e162]
        - separator [ref=e165]
        - generic [ref=e168]: Label
    - generic [ref=e172]:
      - heading "Selected field options" [level=4] [ref=e174]
      - generic [ref=e176]:
        - generic [ref=e178]:
          - generic [ref=e179]: Field title
          - textbox [ref=e180]: C2
        - generic [ref=e181]:
          - heading "Options in drop down box (3)" [level=4] [ref=e182]
          - generic [ref=e183]:
            - list [ref=e184]:
              - listitem [ref=e185]:
                - generic [ref=e186]:
                  - textbox [ref=e187]: Option 1
                  - generic [ref=e189] [cursor=pointer]:
                    - checkbox "Default" [ref=e190]
                    - text: Default
                  - generic [ref=e191]:
                    - generic "Delete" [ref=e192] [cursor=pointer]: delete
                    - generic "Move down" [ref=e193] [cursor=pointer]: arrow_downward
                    - generic "Move up" [ref=e194] [cursor=pointer]: arrow_upward
              - listitem [ref=e195]:
                - generic [ref=e196]:
                  - textbox [ref=e197]: Option 2
                  - generic [ref=e199] [cursor=pointer]:
                    - checkbox "Default" [ref=e200]
                    - text: Default
                  - generic [ref=e201]:
                    - generic "Delete" [ref=e202] [cursor=pointer]: delete
                    - generic "Move down" [ref=e203] [cursor=pointer]: arrow_downward
                    - generic "Move up" [ref=e204] [cursor=pointer]: arrow_upward
              - listitem [ref=e205]:
                - generic [ref=e206]:
                  - textbox [ref=e207]: Option 3
                  - generic [ref=e209] [cursor=pointer]:
                    - checkbox "Default" [ref=e210]
                    - text: Default
                  - generic [ref=e211]:
                    - generic "Delete" [ref=e212] [cursor=pointer]: delete
                    - generic "Move down" [ref=e213] [cursor=pointer]: arrow_downward
                    - generic "Move up" [ref=e214] [cursor=pointer]: arrow_upward
            - generic [ref=e215]:
              - button "Add item" [ref=e216] [cursor=pointer]
              - button "Sort A-Z" [ref=e217] [cursor=pointer]
        - generic [ref=e218]: + List import
        - heading "Add to emails" [level=4] [ref=e219]
        - generic [ref=e221] [cursor=pointer]:
          - checkbox "Add this field on New customer emails" [ref=e222]
          - text: Add this field on New customer emails
        - generic [ref=e224] [cursor=pointer]:
          - checkbox "Add this field on Order emails" [ref=e225]
          - text: Add this field on Order emails
        - generic [ref=e227] [cursor=pointer]:
          - checkbox "Add this field on Quote emails" [ref=e228]
          - text: Add this field on Quote emails
        - generic [ref=e230] [cursor=pointer]:
          - checkbox "Add this field on Credit Request email" [ref=e231]
          - text: Add this field on Credit Request email
        - heading "Mobile settings" [level=4] [ref=e232]
        - generic [ref=e234] [cursor=pointer]:
          - checkbox "Visible on mobile" [checked] [ref=e235]
          - text: Visible on mobile
        - generic [ref=e237] [cursor=pointer]:
          - checkbox "Editable on mobile" [checked] [ref=e238]
          - text: Editable on mobile
        - heading "Other settings" [level=4] [ref=e239]
        - generic [ref=e241] [cursor=pointer]:
          - checkbox "This field must have a value" [ref=e242]
          - text: This field must have a value
        - generic [ref=e244] [cursor=pointer]:
          - checkbox "Can filter on this field" [ref=e245]
          - text: Can filter on this field
        - generic [ref=e247]:
          - generic [ref=e248]: Require comment on selection of
          - listbox [ref=e249]:
            - option [ref=e250]: Option 1
            - option [ref=e251]: Option 2
            - option [ref=e252]: Option 3
          - combobox [ref=e255]:
            - list [ref=e256]:
              - listitem [ref=e257]:
                - textbox [ref=e258]
```

# Test source

```ts
  593 | 		const clickResult = await this.page.evaluate((fieldTitle) => {
  594 | 			const normalized = String(fieldTitle).trim().toLowerCase();
  595 | 
  596 | 			const isVisible = (el) => {
  597 | 				if (!el) return false;
  598 | 				const style = window.getComputedStyle(el);
  599 | 				if (style.display === 'none' || style.visibility === 'hidden') return false;
  600 | 				const rect = el.getBoundingClientRect();
  601 | 				return rect.width > 0 && rect.height > 0;
  602 | 			};
  603 | 
  604 | 			// Locate the field card by its h5 heading (native or role-based).
  605 | 			const headings = Array.from(document.querySelectorAll(
  606 | 				'h5, [role="heading"][aria-level="5"]'
  607 | 			)).filter((el) => el.textContent.trim().toLowerCase() === normalized);
  608 | 
  609 | 			if (!headings.length) return { clicked: false, reason: 'field-heading-not-found' };
  610 | 
  611 | 			const isUpArrow = (el) => {
  612 | 				const bind = String(el.getAttribute('data-bind') || '');
  613 | 				const text = String(el.textContent || '').trim().toLowerCase();
  614 | 				const title = (String(el.getAttribute('title') || '') + ' ' + String(el.getAttribute('data-original-title') || '')).toLowerCase();
  615 | 				if (/moveup|move_up|moveorderup|movefieldup|movecustomfieldup/i.test(bind)) return true;
  616 | 				if (['arrow_upward', 'keyboard_arrow_up', 'expand_less', 'arrow_drop_up', 'north'].includes(text)) return true;
  617 | 				if (/\bmove up\b|\bup\b/.test(title)) return true;
  618 | 				return false;
  619 | 			};
  620 | 
  621 | 			for (const heading of headings) {
  622 | 				// Walk up from the heading to find the card, then locate the up arrow within it.
  623 | 				let node = heading.parentElement;
  624 | 				for (let i = 0; i < 8 && node; i++) {
  625 | 					const candidates = Array.from(node.querySelectorAll('i.material-icons, [role="button"], button, a, i'))
  626 | 						.filter((el) => isUpArrow(el) && isVisible(el) && !heading.contains(el));
  627 | 					if (candidates.length) {
  628 | 						const arrow = candidates[0];
  629 | 						arrow.dispatchEvent(new MouseEvent('mouseenter', { bubbles: true }));
  630 | 						arrow.scrollIntoView({ block: 'center' });
  631 | 						arrow.click();
  632 | 						return { clicked: true };
  633 | 					}
  634 | 					node = node.parentElement;
  635 | 				}
  636 | 			}
  637 | 
  638 | 			return { clicked: false, reason: 'up-arrow-not-found' };
  639 | 		}, title);
  640 | 
  641 | 		if (!clickResult.clicked) {
  642 | 			throw new Error(`Could not click move-up arrow for field '${title}': ${clickResult.reason}.`);
  643 | 		}
  644 | 
  645 | 		await this.page.waitForTimeout(500);
  646 | 	}
  647 | 
  648 | 	async renameCustomerField(currentTitle, newTitle) {
  649 | 		const titlePattern = new RegExp(`^\\s*${this.escapeForRegex(currentTitle)}\\s*$`, 'i');
  650 | 
  651 | 		// Locate the field's label (its card heading) directly.
  652 | 		let label = this.page.getByRole('heading', { name: titlePattern, level: 5 }).last();
  653 | 		if (!await label.count()) {
  654 | 			label = this.page
  655 | 				.locator('h5, [role="heading"][aria-level="5"]')
  656 | 				.filter({ hasText: titlePattern })
  657 | 				.last();
  658 | 		}
  659 | 		if (!await label.count()) {
  660 | 			throw new Error(`Could not find label for customer field '${currentTitle}'.`);
  661 | 		}
  662 | 
  663 | 		await label.scrollIntoViewIfNeeded().catch(() => null);
  664 | 
  665 | 		// Detect whether an inline editor (input/textarea/contenteditable) holding the
  666 | 		// current label text became focused/active after interacting with the label.
  667 | 		const detectInlineEditor = async () => {
  668 | 			return this.page.evaluate((cur) => {
  669 | 				const norm = String(cur).trim().toLowerCase();
  670 | 				const el = document.activeElement;
  671 | 				if (!el) return null;
  672 | 				const tag = (el.tagName || '').toLowerCase();
  673 | 				const isInput = tag === 'input' || tag === 'textarea';
  674 | 				const isEditable = isInput || el.isContentEditable;
  675 | 				if (!isEditable) return null;
  676 | 				const value = isInput ? String(el.value || '') : String(el.textContent || '');
  677 | 				return { editable: true, matches: value.trim().toLowerCase() === norm };
  678 | 			}, currentTitle);
  679 | 		};
  680 | 
  681 | 		// Click the label to enter edit mode; fall back to double-click if needed.
  682 | 		await label.click({ force: true });
  683 | 		await this.page.waitForTimeout(300);
  684 | 		let editor = await detectInlineEditor();
  685 | 
  686 | 		if (!editor || !editor.editable) {
  687 | 			await label.dblclick({ force: true }).catch(() => null);
  688 | 			await this.page.waitForTimeout(300);
  689 | 			editor = await detectInlineEditor();
  690 | 		}
  691 | 
  692 | 		if (!editor || !editor.editable) {
> 693 | 			throw new Error(`Clicking the label for '${currentTitle}' did not open an inline editor.`);
      |          ^ Error: Clicking the label for 'C2' did not open an inline editor.
  694 | 		}
  695 | 
  696 | 		// Edit the label itself: select existing text, replace with the new title, commit.
  697 | 		await this.page.keyboard.press('Control+a');
  698 | 		await this.page.keyboard.press('Delete');
  699 | 		await this.page.keyboard.type(newTitle);
  700 | 		await this.page.keyboard.press('Enter');
  701 | 		await this.page.waitForTimeout(300);
  702 | 	}
  703 | 
  704 | 	async deleteCustomerFieldByLabel(title) {
  705 | 		const normalizedTitle = String(title || '').trim();
  706 | 		if (!normalizedTitle) {
  707 | 			throw new Error('Field title is required when deleting a customer field.');
  708 | 		}
  709 | 
  710 | 		const titlePattern = new RegExp(`^\\s*${this.escapeForRegex(normalizedTitle)}\\s*$`, 'i');
  711 | 
  712 | 		// Select the field first so its delete bin becomes visible.
  713 | 		await this.selectCustomerFieldByTitle(normalizedTitle).catch(() => null);
  714 | 		await this.page.waitForTimeout(400);
  715 | 
  716 | 		// Find the field's card (the ancestor that contains the removeFormItem bin).
  717 | 		let heading = this.page.getByRole('heading', { name: titlePattern, level: 5 }).last();
  718 | 		if (!await heading.count()) {
  719 | 			heading = this.page
  720 | 				.locator('h5, [role="heading"][aria-level="5"]')
  721 | 				.filter({ hasText: titlePattern })
  722 | 				.last();
  723 | 		}
  724 | 
  725 | 		if (!await heading.count()) {
  726 | 			const presentHeadings = await this.page
  727 | 				.locator('h5, [role="heading"][aria-level="5"]')
  728 | 				.allInnerTexts()
  729 | 				.catch(() => []);
  730 | 			console.warn(`[deleteCustomerFieldByLabel] Field '${title}' not found (already deleted?). Present fields: [${presentHeadings.map((t) => t.trim()).filter(Boolean).join(', ')}].`);
  731 | 			return false;
  732 | 		}
  733 | 
  734 | 		await heading.scrollIntoViewIfNeeded().catch(() => null);
  735 | 		await heading.hover({ force: true }).catch(() => null);
  736 | 		await this.page.waitForTimeout(300);
  737 | 
  738 | 		// The delete bin is bound to removeFormItem. Prefer the one inside the field's
  739 | 		// own card; fall back to any visible removeFormItem bin near the selection.
  740 | 		const cardWithBin = heading
  741 | 			.locator('xpath=ancestor::*[.//i[contains(@data-bind,"removeFormItem")]][1]')
  742 | 			.first();
  743 | 
  744 | 		const binCandidates = [
  745 | 			cardWithBin.locator('i[data-bind*="removeFormItem"]').first(),
  746 | 			heading
  747 | 				.locator('xpath=ancestor::*[self::div or self::li or self::section][1]')
  748 | 				.locator('i[data-bind*="removeFormItem"]').first(),
  749 | 			this.page.locator('i[data-bind*="removeFormItem"]:visible').last()
  750 | 		];
  751 | 
  752 | 		// Click the bin once, reliably. This UI often marks the field for deletion
  753 | 		// and keeps the row visible until Save, so we do NOT assert removal here.
  754 | 		const clickBinOnce = async (bin) => {
  755 | 			await bin.scrollIntoViewIfNeeded().catch(() => null);
  756 | 			await bin.hover({ force: true }).catch(() => null);
  757 | 			await this.page.waitForTimeout(150);
  758 | 
  759 | 			// 1) Real Playwright click (trusted, actionable) fires the KO handler.
  760 | 			if (await bin.click({ timeout: 3000 }).then(() => true).catch(() => false)) {
  761 | 				return true;
  762 | 			}
  763 | 
  764 | 			// 2) Coordinate-based mouse click on the bin's center.
  765 | 			const box = await bin.boundingBox().catch(() => null);
  766 | 			if (box) {
  767 | 				await this.page.mouse.move(box.x + box.width / 2, box.y + box.height / 2);
  768 | 				await this.page.mouse.click(box.x + box.width / 2, box.y + box.height / 2);
  769 | 				return true;
  770 | 			}
  771 | 
  772 | 			// 3) Force click (bypass actionability checks).
  773 | 			if (await bin.click({ force: true }).then(() => true).catch(() => false)) {
  774 | 				return true;
  775 | 			}
  776 | 
  777 | 			// 4) Dispatch a native click event directly on the element.
  778 | 			return bin.dispatchEvent('click').then(() => true).catch(() => false);
  779 | 		};
  780 | 
  781 | 		// Clicking the bin triggers a native confirm() dialog ("Are you sure you wish
  782 | 		// to delete..."). Playwright auto-dismisses (Cancel) native dialogs by default,
  783 | 		// which cancels the delete — so accept it (click OK) when it appears.
  784 | 		this.page.once('dialog', (dialog) => dialog.accept().catch(() => null));
  785 | 
  786 | 		let clicked = false;
  787 | 		for (const bin of binCandidates) {
  788 | 			if (!await bin.count().catch(() => 0)) continue;
  789 | 			if (await clickBinOnce(bin)) {
  790 | 				clicked = true;
  791 | 				break;
  792 | 			}
  793 | 		}
```