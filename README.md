# Pipefy SDK

## General

### Constructor

```python
Pipefy(self, token, mock_server=False)
```
Integration class with Pipefy rest api.

## Pipes

### pipe

```python
Pipefy.pipe(self, id, response_fields=None, headers={})
```
Show pipe: Get a pipe by its identifier.

## pipes

```python
Pipefy.pipes(self, ids=[], response_fields=None, headers={})
```
List pipes: Get pipes by their identifiers. 

### createPipe

```python
Pipefy.createPipe(self, organization_id, name, labels=[], members=[], phases=[], start_form_fields=[], preferences={}, response_fields=None, headers={})
```
Create pipe: Mutation to create a pipe, in case of success a query is returned. 

### updatePipeRelation

```python
Pipefy.updatePipeRelation(self, id, name, allChildrenMustBeDoneToFinishParent, childMustExistToMoveParent, childMustExistToFinishParent, allChildrenMustBeDoneToMoveParent, canCreateNewItems, canConnectExistingItems, canConnectMultipleItems, response_fields=None, headers={})
```
Update pipe relation: Mutation to update a pipe relation, in case of success a query is returned. 

### updatePipe

```python
Pipefy.updatePipe(self, id, icon=None, title_field_id=None, public=None, public_form=None, only_assignees_can_edit_cards=None, anyone_can_create_card=None, expiration_time_by_unit=None, expiration_unit=None, response_fields=None, headers={})
```
Update pipe: Mutation to update a pipe, in case of success a query is returned. 

### clonePipes

```python
Pipefy.clonePipes(self, organization_id, pipe_template_ids=[], response_fields=None, headers={})
```
Clone pipe: Mutation to clone a pipe, in case of success a query is returned. 

### pipe_relations

```python
Pipefy.pipe_relations(self, ids, response_fields=None, headers={})
```
Show pipe relations: Get pipe relations by their identifiers. 

### createPipeRelation

```python
Pipefy.createPipeRelation(self, parentId, childId, name, allChildrenMustBeDoneToFinishParent, childMustExistToMoveParent, childMustExistToFinishParent, allChildrenMustBeDoneToMoveParent, canCreateNewItems, canConnectExistingItems, canConnectMultipleItems, response_fields=None, headers={})
```
Create pipe relation: Mutation to create a pipe relation between two pipes, in case of success a query is returned. 

### deletePipeRelation

```python
Pipefy.deletePipeRelation(self, id, response_fields=None, headers={})
```
Delete pipe relation: Mutation to delete a pipe relation, in case of success success: true is returned. 

### deletePipe

```python
Pipefy.deletePipe(self, id, response_fields=None, headers={})
```
Delete pipe: Mutation to delete a pipe, in case of success success: true is returned. 

## Comments

## createComment

```python
Pipefy.createComment(self, card_id, text, response_fields=None, headers={})
```
Create comment: Mutation to create a comment, in case of success a query is returned. 

### updateComment

```python
Pipefy.updateComment(self, id, text, response_fields=None, headers={})
```
Update comment: Mutation to update a comment, in case of success a query is returned. 

## deleteComment

```python
Pipefy.deleteComment(self, id, response_fields=None, headers={})
```
Delete comment: Mutation to delete a comment, in case of success success: true is returned. 

## Phase

### phase

```python
Pipefy.phase(self, id, response_fields=None, headers={})
```
Show phase: Get a phase by its identifier. 

### createPhase

```python
Pipefy.createPhase(self, pipe_id, name, done, lateness_time, description, can_receive_card_directly_from_draft, response_fields=None, headers={})
```
Create phase: Mutation to create a phase, in case of success a query is returned. 

### createPhaseField

```python
Pipefy.createPhaseField(self, phase_id, type, label, options, description, required, editable, response_fields=None, headers={})
```
Create phase field: Mutation to create a phase field, in case of success a query is returned. 

### updatePhaseField

```python
Pipefy.updatePhaseField(self, id, label, options, required, editable, response_fields=None, headers={})
```
Update phase field: Mutation to update a phase field, in case of success a query is returned. 

### updatePhase

```python
Pipefy.updatePhase(self, id, name, done, description, can_receive_card_directly_from_draft, response_fields=None, headers={})
```
Update phase: Mutation to update a phase, in case of success a query is returned. 

### deletePhaseField

```python
Pipefy.deletePhaseField(self, id, response_fields=None, headers={})
```
Delete phase field: Mutation to delete a phase field, in case of success success: true is returned. 

### deletePhase

```python
Pipefy.deletePhase(self, id, response_fields=None, headers={})
```
Delete phase: Mutation to delete a phase of a pipe, in case of success success: true is returned. 

## Label

### createLabel

```python
Pipefy.createLabel(self, pipe_id, name, color, response_fields=None, headers={})
```
Create label: Mutation to create a label, in case of success a query is returned. 

### updateLabel

```python
Pipefy.updateLabel(self, id, name, color, response_fields=None, headers={})
```
Update label: Mutation to update a label, in case of success a query is returned.

### deleteLabel

```python
Pipefy.deleteLabel(self, id, response_fields=None, headers={})
```
Delete label: Mutation to delete a label, in case of success success: true is returned. 

## Card

### card

```python
Pipefy.card(self, id, response_fields=None, headers={})
```
Show card: Get a card by its identifier. 

### cards

```python
Pipefy.cards(self, pipe_id, count=10, search={}, response_fields=None, headers={})
```
List cards: Get cards by pipe identifier. 

### allCards

```python
Pipefy.allCards(self, pipe_id, filter="", response_fields=None, headers={})
```
List cards: Get all cards by pipe identifier and specific filters (any field and operators). 

Example of use:

pipefy.allCards("821643",
        filter='{field: "updated_at", operator: gt, value: 2018-08-01T23:50:11-03:00}')

### createCard

```python
Pipefy.createCard(self, pipe_id, fields_attributes, parent_ids=[], response_fields=None, headers={})
```
Create card: Mutation to create a card, in case of success a query is returned. 

### updateCard

```python
Pipefy.updateCard(self, id, title=None, due_date=None, assignee_ids=[], label_ids=[], response_fields=None, headers={})
```
Update card: Mutation to update a card, in case of success a query is returned. 

### updateCardField

```python
Pipefy.updateCardField(self, card_id, field_id, new_value, response_fields=None, headers={})
```
Update card field: Mutation to update a card field, in case of success a query is returned. 

### moveCardToPhase

```python
Pipefy.moveCardToPhase(self, card_id, destination_phase_id, response_fields=None, headers={})
```
Move card to phase: Mutation to move a card to a phase, in case of success a query is returned. 

### deleteCard

```python
Pipefy.deleteCard(self, id, response_fields=None, headers={})
```
Delete card: Mutation to delete a card, in case of success success: true is returned. 

## Role

### setRole

```python
Pipefy.setRole(self, pipe_id, member, response_fields=None, headers={})
```
Set role: Mutation to set a user's role, in case of success a query is returned. 


## Databases

### deleteTableRecord

```python
Pipefy.deleteTableRecord(self, id, response_fields=None, headers={})
```
Delete table record: Mutation to delete a table record, in case of success a query with the field success is returned. 

### updateTable

```python
Pipefy.updateTable(self, id, name, description, public, authorization, icon, create_record_button_label, title_field_id, public_form, summary_attributes, response_fields=None, headers={})
```
Update table: Mutation to update a table, in case of success a query is returned. 

### createTable

```python
Pipefy.createTable(self, organization_id, name, description, public, authorization, response_fields=None, headers={})
```
Create table: Mutation to create a table, in case of success a query is returned. 

### deleteTable

```python
Pipefy.deleteTable(self, id, response_fields=None, headers={})
```
Delete table: Mutation to delete a table, in case of success a query with the field success is returned. 

### updateTableRecord

```python
Pipefy.updateTableRecord(self, id, title, due_date, response_fields=None, headers={})
```
Update table record: Mutation to update a table record, in case of success a query is returned. 

### createTableField

```python
Pipefy.createTableField(self, table_id, type, label, options, description, help, required, minimal_view, custom_validation, response_fields=None, headers={})
```
Create table field: Mutation to create a table field, in case of success a query is returned. 

### table_records

```python
Pipefy.table_records(self, table_id, first=10, response_fields=None, headers={})
```
List table records: Get table records with pagination through table id. 

### createTableRecord

```python
Pipefy.createTableRecord(self, table_id, title='', due_date=None, fields_attributes=[], response_fields=None, headers={})
```
Create table record: Mutation to create a table record, in case of success a query is returned. 

### table_record

```python
Pipefy.table_record(self, id, response_fields=None, headers={})
```
Show table record: Get table record through table record id. 

### tables

```python
Pipefy.tables(self, ids, response_fields=None, headers={})
```
List tables: Get tables through table ids. 

### table

```python
Pipefy.table(self, id, response_fields=None, headers={})
```
Show table: Get a table through table id. 

### deleteTableField

```python
Pipefy.deleteTableField(self, table_id, id, response_fields=None, headers={})
```
Delete table field: Mutation to delete a table field, in case of success a query with the field success is returned. 

### updateTableField

```python
Pipefy.updateTableField(self, table_id, id, label, options, description, help, required, minimal_view, custom_validation, response_fields=None, headers={})
```
Update table field: Mutation to update a table field, in case of success a query is returned. 

### setTableRecordFieldValue

```python
Pipefy.setTableRecordFieldValue(self, table_record_id, field_id, value, response_fields=None, headers={})
```
Set table record field value: Mutation to set a table record field value, in case of success a query with the field success is returned. 

### setTableFieldOrder

```python
Pipefy.setTableFieldOrder(self, table_id, field_ids, response_fields=None, headers={})
```
Set table record field value Mutation to set a table field order, in case of success a query with the field success is returned. 

## Examples

### Get phases from an specific Pipe

To get access to your token access the [Personal Tokens](https://app.pipefy.com/tokens) and generate one.
The pipe id is the number followed by the name of pipe in the URL when the pipe is open, for example, for this URL ```https://app.pipefy.com/pipes/12345``` the id is 12345.
The method ```pipes``` can send a list of pipe ids. The return is the list of _phases_ and related attribues.

```
from pipefy import Pipefy

token = "your_token_here"
pipe_id = <pipe_id>
pipefy = Pipefy(token)

pipes = pipefy.pipes([pipe_id])
print(pipes)
```
