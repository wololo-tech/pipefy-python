<h1 id="pipefy.Pipefy">Pipefy</h1>

```python
Pipefy(self, token, mock_server=False)
```
Integration class with Pipefy rest api. 
<h2 id="pipefy.Pipefy.deletePhaseField">deletePhaseField</h2>

```python
Pipefy.deletePhaseField(self, id, response_fields=None, headers={})
```
Delete phase field: Mutation to delete a phase field, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.updatePipeRelation">updatePipeRelation</h2>

```python
Pipefy.updatePipeRelation(self, id, name, allChildrenMustBeDoneToFinishParent, childMustExistToMoveParent, childMustExistToFinishParent, allChildrenMustBeDoneToMoveParent, canCreateNewItems, canConnectExistingItems, canConnectMultipleItems, response_fields=None, headers={})
```
Update pipe relation: Mutation to update a pipe relation, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.updatePipe">updatePipe</h2>

```python
Pipefy.updatePipe(self, id, icon=None, title_field_id=None, public=None, public_form=None, only_assignees_can_edit_cards=None, anyone_can_create_card=None, expiration_time_by_unit=None, expiration_unit=None, response_fields=None, headers={})
```
Update pipe: Mutation to update a pipe, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.deleteTableRecord">deleteTableRecord</h2>

```python
Pipefy.deleteTableRecord(self, id, response_fields=None, headers={})
```
Delete table record: Mutation to delete a table record, in case of success a query with the field success is returned. 
<h2 id="pipefy.Pipefy.pipe">pipe</h2>

```python
Pipefy.pipe(self, id, response_fields=None, headers={})
```
Show pipe: Get a pipe by its identifier. 
<h2 id="pipefy.Pipefy.updateTable">updateTable</h2>

```python
Pipefy.updateTable(self, id, name, description, public, authorization, icon, create_record_button_label, title_field_id, public_form, summary_attributes, response_fields=None, headers={})
```
Update table: Mutation to update a table, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createPipe">createPipe</h2>

```python
Pipefy.createPipe(self, organization_id, name, labels=[], members=[], phases=[], start_form_fields=[], preferences={}, response_fields=None, headers={})
```
Create pipe: Mutation to create a pipe, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.deleteComment">deleteComment</h2>

```python
Pipefy.deleteComment(self, id, response_fields=None, headers={})
```
Delete comment: Mutation to delete a comment, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.updatePhase">updatePhase</h2>

```python
Pipefy.updatePhase(self, id, name, done, description, can_receive_card_directly_from_draft, response_fields=None, headers={})
```
Update phase: Mutation to update a phase, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createComment">createComment</h2>

```python
Pipefy.createComment(self, card_id, text, response_fields=None, headers={})
```
Create comment: Mutation to create a comment, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createPhase">createPhase</h2>

```python
Pipefy.createPhase(self, pipe_id, name, done, lateness_time, description, can_receive_card_directly_from_draft, response_fields=None, headers={})
```
Create phase: Mutation to create a phase, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createTable">createTable</h2>

```python
Pipefy.createTable(self, organization_id, name, description, public, authorization, response_fields=None, headers={})
```
Create table: Mutation to create a table, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.updateLabel">updateLabel</h2>

```python
Pipefy.updateLabel(self, id, name, color, response_fields=None, headers={})
```
Update label: Mutation to update a label, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.deleteCard">deleteCard</h2>

```python
Pipefy.deleteCard(self, id, response_fields=None, headers={})
```
Delete card: Mutation to delete a card, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.pipe_relations">pipe_relations</h2>

```python
Pipefy.pipe_relations(self, ids, response_fields=None, headers={})
```
Show pipe relations: Get pipe relations by their identifiers. 
<h2 id="pipefy.Pipefy.card">card</h2>

```python
Pipefy.card(self, id, response_fields=None, headers={})
```
Show card: Get a card by its identifier. 
<h2 id="pipefy.Pipefy.deletePipeRelation">deletePipeRelation</h2>

```python
Pipefy.deletePipeRelation(self, id, response_fields=None, headers={})
```
Delete pipe relation: Mutation to delete a pipe relation, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.deleteTable">deleteTable</h2>

```python
Pipefy.deleteTable(self, id, response_fields=None, headers={})
```
Delete table: Mutation to delete a table, in case of success a query with the field success is returned. 
<h2 id="pipefy.Pipefy.createCard">createCard</h2>

```python
Pipefy.createCard(self, pipe_id, fields_attributes, parent_ids=[], response_fields=None, headers={})
```
Create card: Mutation to create a card, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.moveCardToPhase">moveCardToPhase</h2>

```python
Pipefy.moveCardToPhase(self, card_id, destination_phase_id, response_fields=None, headers={})
```
Move card to phase: Mutation to move a card to a phase, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.clonePipes">clonePipes</h2>

```python
Pipefy.clonePipes(self, organization_id, pipe_template_ids=[], response_fields=None, headers={})
```
Clone pipe: Mutation to clone a pipe, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.updatePhaseField">updatePhaseField</h2>

```python
Pipefy.updatePhaseField(self, id, label, options, required, editable, response_fields=None, headers={})
```
Update phase field: Mutation to update a phase field, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.updateCardField">updateCardField</h2>

```python
Pipefy.updateCardField(self, card_id, field_id, new_value, response_fields=None, headers={})
```
Update card field: Mutation to update a card field, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.updateTableRecord">updateTableRecord</h2>

```python
Pipefy.updateTableRecord(self, id, title, due_date, response_fields=None, headers={})
```
Update table record: Mutation to update a table record, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createTableField">createTableField</h2>

```python
Pipefy.createTableField(self, table_id, type, label, options, description, help, required, minimal_view, custom_validation, response_fields=None, headers={})
```
Create table field: Mutation to create a table field, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createLabel">createLabel</h2>

```python
Pipefy.createLabel(self, pipe_id, name, color, response_fields=None, headers={})
```
Create label: Mutation to create a label, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createPipeRelation">createPipeRelation</h2>

```python
Pipefy.createPipeRelation(self, parentId, childId, name, allChildrenMustBeDoneToFinishParent, childMustExistToMoveParent, childMustExistToFinishParent, allChildrenMustBeDoneToMoveParent, canCreateNewItems, canConnectExistingItems, canConnectMultipleItems, response_fields=None, headers={})
```
Create pipe relation: Mutation to create a pipe relation between two pipes, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.table_records">table_records</h2>

```python
Pipefy.table_records(self, table_id, first=10, response_fields=None, headers={})
```
List table records: Get table records with pagination through table id. 
<h2 id="pipefy.Pipefy.setRole">setRole</h2>

```python
Pipefy.setRole(self, pipe_id, member, response_fields=None, headers={})
```
Set role: Mutation to set a user's role, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.createPhaseField">createPhaseField</h2>

```python
Pipefy.createPhaseField(self, phase_id, type, label, options, description, required, editable, response_fields=None, headers={})
```
Create phase field: Mutation to create a phase field, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.deleteLabel">deleteLabel</h2>

```python
Pipefy.deleteLabel(self, id, response_fields=None, headers={})
```
Delete label: Mutation to delete a label, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.updateCard">updateCard</h2>

```python
Pipefy.updateCard(self, id, title=None, due_date=None, assignee_ids=[], label_ids=[], response_fields=None, headers={})
```
Update card: Mutation to update a card, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.pipes">pipes</h2>

```python
Pipefy.pipes(self, ids=[], response_fields=None, headers={})
```
List pipes: Get pipes by their identifiers. 
<h2 id="pipefy.Pipefy.createTableRecord">createTableRecord</h2>

```python
Pipefy.createTableRecord(self, table_id, title='', due_date=None, fields_attributes=[], response_fields=None, headers={})
```
Create table record: Mutation to create a table record, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.table_record">table_record</h2>

```python
Pipefy.table_record(self, id, response_fields=None, headers={})
```
Show table record: Get table record through table record id. 
<h2 id="pipefy.Pipefy.cards">cards</h2>

```python
Pipefy.cards(self, pipe_id, count=10, search={}, response_fields=None, headers={})
```
List cards: Get cards by pipe identifier. 
<h2 id="pipefy.Pipefy.tables">tables</h2>

```python
Pipefy.tables(self, ids, response_fields=None, headers={})
```
List tables: Get tables through table ids. 
<h2 id="pipefy.Pipefy.deletePhase">deletePhase</h2>

```python
Pipefy.deletePhase(self, id, response_fields=None, headers={})
```
Delete phase: Mutation to delete a phase of a pipe, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.updateComment">updateComment</h2>

```python
Pipefy.updateComment(self, id, text, response_fields=None, headers={})
```
Update comment: Mutation to update a comment, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.table">table</h2>

```python
Pipefy.table(self, id, response_fields=None, headers={})
```
Show table: Get a table through table id. 
<h2 id="pipefy.Pipefy.deleteTableField">deleteTableField</h2>

```python
Pipefy.deleteTableField(self, table_id, id, response_fields=None, headers={})
```
Delete table field: Mutation to delete a table field, in case of success a query with the field success is returned. 
<h2 id="pipefy.Pipefy.deletePipe">deletePipe</h2>

```python
Pipefy.deletePipe(self, id, response_fields=None, headers={})
```
Delete pipe: Mutation to delete a pipe, in case of success success: true is returned. 
<h2 id="pipefy.Pipefy.updateTableField">updateTableField</h2>

```python
Pipefy.updateTableField(self, table_id, id, label, options, description, help, required, minimal_view, custom_validation, response_fields=None, headers={})
```
Update table field: Mutation to update a table field, in case of success a query is returned. 
<h2 id="pipefy.Pipefy.setTableRecordFieldValue">setTableRecordFieldValue</h2>

```python
Pipefy.setTableRecordFieldValue(self, table_record_id, field_id, value, response_fields=None, headers={})
```
Set table record field value: Mutation to set a table record field value, in case of success a query with the field success is returned. 
<h2 id="pipefy.Pipefy.phase">phase</h2>

```python
Pipefy.phase(self, id, response_fields=None, headers={})
```
Show phase: Get a phase by its identifier. 
<h2 id="pipefy.Pipefy.setTableFieldOrder">setTableFieldOrder</h2>

```python
Pipefy.setTableFieldOrder(self, table_id, field_ids, response_fields=None, headers={})
```
Set table record field value Mutation to set a table field order, in case of success a query with the field success is returned. 
