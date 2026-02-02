# Reference
## Comments
<details><summary><code>client.comments.list(landscapeId, versionId) -> CommentsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().list(
    "landscapeId",
    "versionId",
    CommentsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**status:** `Optional<String>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.create(landscapeId, versionId, request) -> CommentsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().create(
    "landscapeId",
    "versionId",
    CommentCreateRequest
        .builder()
        .body(
            CommentRequired
                .builder()
                .body(
                    CommentBody.of(
                        CommentBodyQuestion
                            .builder()
                            .content("content")
                            .status(CommentBodyQuestionStatus.OPEN)
                            .type(CommentBodyQuestionType.QUESTION)
                            .build()
                    )
                )
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CommentRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.get(landscapeId, versionId, commentId) -> CommentsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().get(
    "landscapeId",
    "versionId",
    "commentId",
    CommentFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.upsert(landscapeId, versionId, commentId, request) -> CommentsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().upsert(
    "landscapeId",
    "versionId",
    "commentId",
    CommentUpsertRequest
        .builder()
        .body(
            CommentUpsert
                .builder()
                .body(
                    CommentBody.of(
                        CommentBodyQuestion
                            .builder()
                            .content("content")
                            .status(CommentBodyQuestionStatus.OPEN)
                            .type(CommentBodyQuestionType.QUESTION)
                            .build()
                    )
                )
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CommentUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.delete(landscapeId, versionId, commentId) -> CommentsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().delete(
    "landscapeId",
    "versionId",
    "commentId",
    CommentDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.update(landscapeId, versionId, commentId, request) -> CommentsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().update(
    "landscapeId",
    "versionId",
    "commentId",
    CommentUpdateRequest
        .builder()
        .body(
            CommentPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CommentPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Diagrams
<details><summary><code>client.diagrams.list(landscapeId, versionId) -> DiagramsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().list(
    "landscapeId",
    "versionId",
    DiagramsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<DiagramFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.create(landscapeId, versionId, request) -> DiagramsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().create(
    "landscapeId",
    "versionId",
    DiagramCreateRequest
        .builder()
        .body(
            DiagramCreate
                .builder()
                .index(1.1)
                .modelId("modelId")
                .name("name")
                .type(DiagramType.APP_DIAGRAM)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramCreate` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.get(landscapeId, versionId, diagramId) -> DiagramsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().get(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.upsert(landscapeId, versionId, diagramId, request) -> DiagramsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().upsert(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramUpsertRequest
        .builder()
        .body(
            DiagramCreate
                .builder()
                .index(1.1)
                .modelId("modelId")
                .name("name")
                .type(DiagramType.APP_DIAGRAM)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramCreate` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.delete(landscapeId, versionId, diagramId) -> DiagramsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().delete(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.update(landscapeId, versionId, diagramId, request) -> DiagramsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().update(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramUpdateRequest
        .builder()
        .body(
            DiagramUpsert
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.exists(landscapeId, versionId, diagramId)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().exists(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramExistsRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.listThumbnails(landscapeId, versionId) -> DiagramsListThumbnailsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().listThumbnails(
    "landscapeId",
    "versionId",
    DiagramThumbnailsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<DiagramFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.getThumbnail(landscapeId, versionId, diagramId) -> DiagramsGetThumbnailResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().getThumbnail(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramThumbnailGetRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Domains
<details><summary><code>client.domains.list(landscapeId, versionId) -> DomainsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().list(
    "landscapeId",
    "versionId",
    DomainsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<DomainFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.domains.create(landscapeId, versionId, request) -> DomainsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().create(
    "landscapeId",
    "versionId",
    DomainCreateRequest
        .builder()
        .body(
            DomainRequired
                .builder()
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DomainRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.domains.get(landscapeId, versionId, domainId) -> DomainsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().get(
    "landscapeId",
    "versionId",
    "domainId",
    DomainFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**domainId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.domains.upsert(landscapeId, versionId, domainId, request) -> DomainsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().upsert(
    "landscapeId",
    "versionId",
    "domainId",
    DomainUpsertRequest
        .builder()
        .body(
            DomainUpsert
                .builder()
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**domainId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DomainUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.domains.delete(landscapeId, versionId, domainId) -> DomainsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().delete(
    "landscapeId",
    "versionId",
    "domainId",
    DomainDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**domainId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.domains.update(landscapeId, versionId, domainId, request) -> DomainsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().update(
    "landscapeId",
    "versionId",
    "domainId",
    DomainUpdateRequest
        .builder()
        .body(
            DomainPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**domainId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DomainPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.domains.exists(landscapeId, versionId, domainId)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.domains().exists(
    "landscapeId",
    "versionId",
    "domainId",
    DomainExistsRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**domainId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Drafts
<details><summary><code>client.drafts.list(landscapeId, versionId) -> DraftsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().list(
    "landscapeId",
    "versionId",
    DraftsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<DraftFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.drafts.create(landscapeId, versionId, request) -> DraftsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().create(
    "landscapeId",
    "versionId",
    DraftCreateRequest
        .builder()
        .body(
            DraftRequired
                .builder()
                .name("name")
                .status(DraftStatus.IN_PROGRESS)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DraftRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.drafts.get(landscapeId, versionId, draftId) -> DraftsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().get(
    "landscapeId",
    "versionId",
    "draftId",
    DraftFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**draftId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.drafts.upsert(landscapeId, versionId, draftId, request) -> DraftsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().upsert(
    "landscapeId",
    "versionId",
    "draftId",
    DraftUpsertRequest
        .builder()
        .body(
            DraftRequired
                .builder()
                .name("name")
                .status(DraftStatus.IN_PROGRESS)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**draftId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DraftRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.drafts.delete(landscapeId, versionId, draftId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().delete(
    "landscapeId",
    "versionId",
    "draftId",
    DraftDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**draftId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.drafts.update(landscapeId, versionId, draftId, request) -> DraftsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().update(
    "landscapeId",
    "versionId",
    "draftId",
    DraftUpdateRequest
        .builder()
        .body(
            DraftPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**draftId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DraftPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.drafts.merge(landscapeId, versionId, draftId) -> DraftsMergeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.drafts().merge(
    "landscapeId",
    "versionId",
    "draftId",
    DraftMergeRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**draftId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Flows
<details><summary><code>client.flows.list(landscapeId, versionId) -> FlowsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().list(
    "landscapeId",
    "versionId",
    FlowsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<FlowFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.create(landscapeId, versionId, request) -> FlowsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().create(
    "landscapeId",
    "versionId",
    FlowCreateRequest
        .builder()
        .body(
            FlowRequired
                .builder()
                .name("name")
                .diagramId("diagramId")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `FlowRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.get(landscapeId, versionId, flowId) -> FlowsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().get(
    "landscapeId",
    "versionId",
    "flowId",
    FlowFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.upsert(landscapeId, versionId, flowId, request) -> FlowsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().upsert(
    "landscapeId",
    "versionId",
    "flowId",
    FlowUpsertRequest
        .builder()
        .body(
            FlowRequired
                .builder()
                .name("name")
                .diagramId("diagramId")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `FlowRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.delete(landscapeId, versionId, flowId) -> FlowsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().delete(
    "landscapeId",
    "versionId",
    "flowId",
    FlowDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.update(landscapeId, versionId, flowId, request) -> FlowsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().update(
    "landscapeId",
    "versionId",
    "flowId",
    FlowUpdateRequest
        .builder()
        .body(
            FlowPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `FlowPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.exists(landscapeId, versionId, flowId)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().exists(
    "landscapeId",
    "versionId",
    "flowId",
    FlowExistsRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.listThumbnails(landscapeId, versionId) -> FlowsListThumbnailsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().listThumbnails(
    "landscapeId",
    "versionId",
    FlowThumbnailsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<DiagramFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.getThumbnail(landscapeId, versionId, flowId) -> FlowsGetThumbnailResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().getThumbnail(
    "landscapeId",
    "versionId",
    "flowId",
    FlowThumbnailGetRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Landscapes
<details><summary><code>client.landscapes.get(landscapeId) -> LandscapesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().get(
    "landscapeId",
    LandscapeFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.delete(landscapeId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().delete(
    "landscapeId",
    LandscapeDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.update(landscapeId, request) -> LandscapesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().update(
    "landscapeId",
    LandscapeUpdateRequest
        .builder()
        .body(
            LandscapePartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `LandscapePartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.duplicate(landscapeId, request) -> LandscapesDuplicateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().duplicate(
    "landscapeId",
    LandscapeDuplicateRequest
        .builder()
        .body(
            LandscapeRequired
                .builder()
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**targetOrganizationId:** `Optional<String>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `LandscapeRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.copy(landscapeId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().copy(
    "landscapeId",
    LandscapeCopyRequest
        .builder()
        .targetLandscapeId("targetLandscapeId")
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**targetLandscapeId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.search(landscapeId, versionId) -> LandscapesSearchResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Search the entire landscape
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().search(
    "landscapeId",
    "versionId",
    LandscapeSearchRequest
        .builder()
        .search("search")
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**search:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<SearchFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**includeData:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**maxResults:** `Optional<Double>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations
<details><summary><code>client.organizations.list() -> OrganizationsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().list(
    OrganizationsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**admin:** `Optional<Boolean>` — list all organizations on the platform
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.create(request) -> OrganizationsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().create(
    OrganizationRequired
        .builder()
        .name("name")
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `OrganizationRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.get(organizationId) -> OrganizationsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().get(
    "organizationId",
    OrganizationFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.delete(organizationId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().delete(
    "organizationId",
    OrganizationDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.update(organizationId, request) -> OrganizationsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().update(
    "organizationId",
    OrganizationUpdateRequest
        .builder()
        .body(
            OrganizationPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `OrganizationPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## ShareLink
<details><summary><code>client.shareLink.get(landscapeId, versionId) -> ShareLinkGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.shareLink().get(
    "landscapeId",
    "versionId",
    ShareLinkFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.shareLink.create(landscapeId, versionId, request) -> ShareLinkCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.shareLink().create(
    "landscapeId",
    "versionId",
    ShareLinkCreateRequest
        .builder()
        .body(
            ShareLinkRequired
                .builder()
                .protected_(true)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ShareLinkRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.shareLink.delete(landscapeId, versionId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.shareLink().delete(
    "landscapeId",
    "versionId",
    ShareLinkDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.shareLink.update(landscapeId, versionId, request) -> ShareLinkUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.shareLink().update(
    "landscapeId",
    "versionId",
    ShareLinkUpdateRequest
        .builder()
        .body(
            ShareLinkPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**resetShortId:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ShareLinkPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Tags
<details><summary><code>client.tags.list(landscapeId, versionId) -> TagsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().list(
    "landscapeId",
    "versionId",
    TagsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<TagFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.create(landscapeId, versionId, request) -> TagsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().create(
    "landscapeId",
    "versionId",
    TagCreateRequest
        .builder()
        .body(
            TagRequired
                .builder()
                .color(TagColor.BLUE)
                .groupId("groupId")
                .index(1.1)
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TagRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.get(landscapeId, versionId, tagId) -> TagsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().get(
    "landscapeId",
    "versionId",
    "tagId",
    TagFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.upsert(landscapeId, versionId, tagId, request) -> TagsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().upsert(
    "landscapeId",
    "versionId",
    "tagId",
    TagUpsertRequest
        .builder()
        .body(
            TagUpsert
                .builder()
                .color(TagColor.BLUE)
                .groupId("groupId")
                .index(1.1)
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TagUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.delete(landscapeId, versionId, tagId) -> TagsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().delete(
    "landscapeId",
    "versionId",
    "tagId",
    TagDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.update(landscapeId, versionId, tagId, request) -> TagsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().update(
    "landscapeId",
    "versionId",
    "tagId",
    TagUpdateRequest
        .builder()
        .body(
            TagPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TagPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Teams
<details><summary><code>client.teams.list(organizationId) -> TeamsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().list(
    "organizationId",
    TeamsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.teams.create(organizationId, request) -> TeamsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().create(
    "organizationId",
    TeamCreateRequest
        .builder()
        .body(
            TeamRequired
                .builder()
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TeamRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.teams.get(organizationId, teamId) -> TeamsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().get(
    "organizationId",
    "teamId",
    TeamFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**teamId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.teams.delete(organizationId, teamId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().delete(
    "organizationId",
    "teamId",
    TeamDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**teamId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.teams.update(organizationId, teamId, request) -> TeamsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().update(
    "organizationId",
    "teamId",
    TeamUpdateRequest
        .builder()
        .body(
            TeamPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**teamId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TeamPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.teams.listLandscapes(organizationId, teamId) -> TeamsListLandscapesResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().listLandscapes(
    "organizationId",
    "teamId",
    TeamLandscapesListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**teamId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.teams.listModelObjects(organizationId, teamId) -> TeamsListModelObjectsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.teams().listModelObjects(
    "organizationId",
    "teamId",
    TeamModelObjectsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**teamId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Versions
<details><summary><code>client.versions.list(landscapeId) -> VersionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().list(
    "landscapeId",
    VersionsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.create(landscapeId, request) -> VersionsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().create(
    "landscapeId",
    VersionCreateRequest
        .builder()
        .body(
            VersionRequired
                .builder()
                .name("name")
                .notes("notes")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `VersionRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.get(landscapeId, versionId) -> VersionsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().get(
    "landscapeId",
    "versionId",
    VersionFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.delete(landscapeId, versionId) -> Object</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().delete(
    "landscapeId",
    "versionId",
    VersionDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.update(landscapeId, versionId, request) -> VersionsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().update(
    "landscapeId",
    "versionId",
    VersionUpdateRequest
        .builder()
        .body(
            VersionPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `VersionPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Catalog Technologies
<details><summary><code>client.catalog.technologies.list() -> TechnologiesListResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List technologies
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.catalog().technologies().list(
    CatalogTechnologiesListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**filter:** `Optional<CatalogTechnologyFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**admin:** `Optional<Boolean>` — list all technologies on the platform
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.technologies.suggestInformation() -> TechnologiesSuggestInformationResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate suggestions for a technologies information
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.catalog().technologies().suggestInformation(
    CatalogSuggestionInformationGetRequest
        .builder()
        .url("url")
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**url:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.technologies.suggestBrand() -> TechnologiesSuggestBrandResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate suggestions for a technologies branding
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.catalog().technologies().suggestBrand(
    CatalogSuggestionBrandGetRequest
        .builder()
        .url("url")
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**url:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.technologies.createSignedIconUrl() -> TechnologiesCreateSignedIconUrlResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a signed URL prefix with access to all catalog icons
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.catalog().technologies().createSignedIconUrl();
```
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.technologies.get(catalogTechnologyId) -> TechnologiesGetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Find a technology
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.catalog().technologies().get(
    "catalogTechnologyId",
    CatalogTechnologyFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**catalogTechnologyId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.catalog.technologies.getSlug(catalogTechnologySlug) -> TechnologiesGetSlugResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Find a technology by the slug
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.catalog().technologies().getSlug(
    "catalogTechnologySlug",
    CatalogTechnologySlugFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**catalogTechnologySlug:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Comments Replies
<details><summary><code>client.comments.replies.list(landscapeId, versionId, commentId) -> RepliesListResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List comment replies
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().replies().list(
    "landscapeId",
    "versionId",
    "commentId",
    CommentRepliesListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.replies.create(landscapeId, versionId, commentId, request) -> RepliesCreateResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Create a comment reply
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().replies().create(
    "landscapeId",
    "versionId",
    "commentId",
    CommentReplyCreateRequest
        .builder()
        .body(
            CommentReplyRequired
                .builder()
                .content("content")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CommentReplyRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.replies.get(landscapeId, versionId, commentId, commentReplyId) -> RepliesGetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Find a comment reply
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().replies().get(
    "landscapeId",
    "versionId",
    "commentId",
    "commentReplyId",
    CommentReplyFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentReplyId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.replies.upsert(landscapeId, versionId, commentId, commentReplyId, request) -> RepliesUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().replies().upsert(
    "landscapeId",
    "versionId",
    "commentId",
    "commentReplyId",
    CommentReplyUpsertRequest
        .builder()
        .body(
            CommentReplyUpsert
                .builder()
                .content("content")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentReplyId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CommentReplyUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.replies.delete(landscapeId, versionId, commentId, commentReplyId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Delete a comment reply
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().replies().delete(
    "landscapeId",
    "versionId",
    "commentId",
    "commentReplyId",
    CommentReplyDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentReplyId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.comments.replies.update(landscapeId, versionId, commentId, commentReplyId, request) -> RepliesUpdateResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Update a comment reply
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.comments().replies().update(
    "landscapeId",
    "versionId",
    "commentId",
    "commentReplyId",
    CommentReplyUpdateRequest
        .builder()
        .body(
            CommentReplyPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**commentReplyId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CommentReplyPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Diagrams Content
<details><summary><code>client.diagrams.content.generateDescription(landscapeId, versionId, diagramId, request) -> ContentGenerateDescriptionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate a description for a diagram
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().content().generateDescription(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramContentGenerateDescriptionRequest
        .builder()
        .type(AiDescriptionType.CAPTION)
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `AiDescriptionType` — Type of description to generate: "caption" for a short caption(50-70 characters), or "detailed" for a detailed description (max 2000 characters)
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.content.get(landscapeId, versionId, diagramId) -> ContentGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().content().get(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramContentFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.content.replace(landscapeId, versionId, diagramId, request) -> ContentReplaceResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().content().replace(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramContentReplaceRequest
        .builder()
        .body(
            DiagramContentRequired
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramContentRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.content.update(landscapeId, versionId, diagramId, request) -> ContentUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().content().update(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramContentUpdateRequest
        .builder()
        .body(
            DiagramContentPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateViewedAt:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramContentPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Diagrams Groups
<details><summary><code>client.diagrams.groups.list(landscapeId, versionId) -> GroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().list(
    "landscapeId",
    "versionId",
    DiagramGroupsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<DiagramGroupFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.groups.create(landscapeId, versionId, request) -> GroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().create(
    "landscapeId",
    "versionId",
    DiagramGroupCreateRequest
        .builder()
        .body(
            DiagramGroupRequired
                .builder()
                .modelId("modelId")
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramGroupRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.groups.get(landscapeId, versionId, diagramGroupId) -> GroupsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().get(
    "landscapeId",
    "versionId",
    "diagramGroupId",
    DiagramGroupFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramGroupId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.groups.upsert(landscapeId, versionId, diagramGroupId, request) -> GroupsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().upsert(
    "landscapeId",
    "versionId",
    "diagramGroupId",
    DiagramGroupUpsertRequest
        .builder()
        .body(
            DiagramGroupUpsert
                .builder()
                .modelId("modelId")
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramGroupId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramGroupUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.groups.delete(landscapeId, versionId, diagramGroupId) -> GroupsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().delete(
    "landscapeId",
    "versionId",
    "diagramGroupId",
    DiagramGroupDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramGroupId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.groups.update(landscapeId, versionId, diagramGroupId, request) -> GroupsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().update(
    "landscapeId",
    "versionId",
    "diagramGroupId",
    DiagramGroupUpdateRequest
        .builder()
        .body(
            DiagramGroupPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramGroupId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramGroupPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.groups.exists(landscapeId, versionId, diagramGroupId)</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().groups().exists(
    "landscapeId",
    "versionId",
    "diagramGroupId",
    DiagramGroupExistsRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramGroupId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Diagrams Export
<details><summary><code>client.diagrams.export.get(landscapeId, versionId, diagramId, diagramExportImageId) -> ExportGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().export().get(
    "landscapeId",
    "versionId",
    "diagramId",
    "diagramExportImageId",
    DiagramExportImageFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramExportImageId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.diagrams.export.create(landscapeId, versionId, diagramId, request) -> ExportCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.diagrams().export().create(
    "landscapeId",
    "versionId",
    "diagramId",
    DiagramExportImageCreateRequest
        .builder()
        .body(
            DiagramExportImageOptions
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**diagramId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `DiagramExportImageOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Flows Export
<details><summary><code>client.flows.export.text(landscapeId, versionId, flowId) -> String</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().export().text(
    "landscapeId",
    "versionId",
    "flowId",
    FlowExportTextRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.export.code(landscapeId, versionId, flowId) -> String</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().export().code(
    "landscapeId",
    "versionId",
    "flowId",
    FlowExportCodeRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.flows.export.mermaid(landscapeId, versionId, flowId) -> String</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.flows().export().mermaid(
    "landscapeId",
    "versionId",
    "flowId",
    FlowExportMermaidRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**flowId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Landscapes Logs
<details><summary><code>client.landscapes.logs.list(landscapeId) -> LogsListResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List action logs
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().logs().list(
    "landscapeId",
    ActionLogsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<ActionLogFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.logs.get(landscapeId, actionLogId) -> LogsGetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Find an action log
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().logs().get(
    "landscapeId",
    "actionLogId",
    ActionLogFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**actionLogId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.logs.listChildren(landscapeId, actionLogId) -> LogsListChildrenResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List actions that happened as a result of a different action
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().logs().listChildren(
    "landscapeId",
    "actionLogId",
    ActionLogChildrenListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**actionLogId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<ActionLogFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Landscapes Export
<details><summary><code>client.landscapes.export.create(landscapeId, versionId, request) -> ExportCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().export().create(
    "landscapeId",
    "versionId",
    LandscapeExportRequest
        .builder()
        .type(LandscapeExportType.PDF)
        .body(
            LandscapeExportOptions
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `LandscapeExportType` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<LandscapeExportFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `LandscapeExportOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.export.get(landscapeId, versionId, landscapeExportId) -> ExportGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().export().get(
    "landscapeId",
    "versionId",
    "landscapeExportId",
    LandscapeExportFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**landscapeExportId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Landscapes Logs Stats
<details><summary><code>client.landscapes.logs.stats.byType(landscapeId) -> ActionLogStatsListByType</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List total counts of actions for each action type (e.g. diagram-content-update, model-object-create)
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().logs().stats().byType(
    "landscapeId",
    ActionLogStatsByTypeRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<ActionLogStatsFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**period:** `Optional<ActionLogStatsPeriod>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.landscapes.logs.stats.byEntity(landscapeId) -> ActionLogStatsListByEntity</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List total counts of actions for each entity identifier
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.landscapes().logs().stats().byEntity(
    "landscapeId",
    ActionLogStatsByEntityRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<ActionLogStatsFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**period:** `Optional<ActionLogStatsPeriod>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Model Connections
<details><summary><code>client.model.connections.list(landscapeId, versionId) -> ConnectionsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().list(
    "landscapeId",
    "versionId",
    ModelConnectionsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<ModelConnectionFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**expand:** `Optional<ModelConnectionExpandKey>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.connections.create(landscapeId, versionId, request) -> ConnectionsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().create(
    "landscapeId",
    "versionId",
    ModelConnectionCreateRequest
        .builder()
        .body(
            ModelConnectionRequired
                .builder()
                .name("name")
                .originId("originId")
                .targetId("targetId")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ModelConnectionRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.connections.get(landscapeId, versionId, modelConnectionId) -> ConnectionsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().get(
    "landscapeId",
    "versionId",
    "modelConnectionId",
    ModelConnectionFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelConnectionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**expand:** `Optional<ModelConnectionExpandKey>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.connections.upsert(landscapeId, versionId, modelConnectionId, request) -> ConnectionsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().upsert(
    "landscapeId",
    "versionId",
    "modelConnectionId",
    ModelConnectionUpsertRequest
        .builder()
        .body(
            ModelConnectionUpsert
                .builder()
                .name("name")
                .originId("originId")
                .targetId("targetId")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelConnectionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**originConnector:** `Optional<ConnectionsUpsertRequestOriginConnector>` 
    
</dd>
</dl>

<dl>
<dd>

**targetConnector:** `Optional<ConnectionsUpsertRequestTargetConnector>` 
    
</dd>
</dl>

<dl>
<dd>

**updateDiagrams:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ModelConnectionUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.connections.delete(landscapeId, versionId, modelConnectionId) -> ConnectionsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().delete(
    "landscapeId",
    "versionId",
    "modelConnectionId",
    ModelConnectionDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelConnectionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.connections.update(landscapeId, versionId, modelConnectionId, request) -> ConnectionsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().update(
    "landscapeId",
    "versionId",
    "modelConnectionId",
    ModelConnectionUpdateRequest
        .builder()
        .body(
            ModelConnectionPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelConnectionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**updateDiagrams:** `Optional<Boolean>` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ModelConnectionPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.connections.generateDescription(landscapeId, versionId, modelConnectionId, request) -> ConnectionsGenerateDescriptionResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Generate a description for a model connection
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().generateDescription(
    "landscapeId",
    "versionId",
    "modelConnectionId",
    ModelConnectionGenerateDescriptionRequest
        .builder()
        .type(AiDescriptionType.CAPTION)
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelConnectionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**type:** `AiDescriptionType` — Type of description to generate: "caption" for a short caption(50-70 characters), or "detailed" for a detailed description (max 2000 characters)
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Model Objects
<details><summary><code>client.model.objects.list(landscapeId, versionId) -> ObjectsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().list(
    "landscapeId",
    "versionId",
    ModelObjectsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<ModelObjectFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**expand:** `Optional<ModelObjectExpandKey>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.objects.create(landscapeId, versionId, request) -> ObjectsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().create(
    "landscapeId",
    "versionId",
    ModelObjectCreateRequest
        .builder()
        .body(
            ModelObjectRequired
                .builder()
                .name("name")
                .type(ModelObjectType.ACTOR)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ModelObjectRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.objects.get(landscapeId, versionId, modelObjectId) -> ObjectsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().get(
    "landscapeId",
    "versionId",
    "modelObjectId",
    ModelObjectFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelObjectId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**expand:** `Optional<ModelObjectExpandKey>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.objects.upsert(landscapeId, versionId, modelObjectId, request) -> ObjectsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().upsert(
    "landscapeId",
    "versionId",
    "modelObjectId",
    ModelObjectUpsertRequest
        .builder()
        .body(
            ModelObjectUpsert
                .builder()
                .name("name")
                .type(ModelObjectType.ACTOR)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelObjectId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ModelObjectUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.objects.delete(landscapeId, versionId, modelObjectId) -> ObjectsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().delete(
    "landscapeId",
    "versionId",
    "modelObjectId",
    ModelObjectDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelObjectId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.objects.update(landscapeId, versionId, modelObjectId, request) -> ObjectsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().update(
    "landscapeId",
    "versionId",
    "modelObjectId",
    ModelObjectUpdateRequest
        .builder()
        .body(
            ModelObjectPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelObjectId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `ModelObjectPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Model Connections Export
<details><summary><code>client.model.connections.export.csv(landscapeId, versionId) -> String</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().connections().export().csv(
    "landscapeId",
    "versionId",
    ModelConnectionsExportCsvRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Model Objects Export
<details><summary><code>client.model.objects.export.dependenciesJson(landscapeId, versionId, modelObjectId) -> ModelObjectDependenciesExport</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Export object dependencies as JSON
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().export().dependenciesJson(
    "landscapeId",
    "versionId",
    "modelObjectId",
    ModelObjectDependenciesExportJsonRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**modelObjectId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.model.objects.export.csv(landscapeId, versionId) -> String</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Export all model objects as CSV
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.model().objects().export().csv(
    "landscapeId",
    "versionId",
    ModelObjectsExportCsvRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations Landscapes
<details><summary><code>client.organizations.landscapes.list(organizationId) -> LandscapesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().landscapes().list(
    "organizationId",
    OrganizationLandscapesListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.landscapes.create(organizationId, request) -> LandscapesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().landscapes().create(
    "organizationId",
    OrganizationLandscapeCreateRequest
        .builder()
        .name("name")
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**templateId:** `Optional<String>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations Logs
<details><summary><code>client.organizations.logs.list(organizationId) -> LogsListResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List organization logs (only available on the scale plan and above)
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().logs().list(
    "organizationId",
    OrganizationLogsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<OrganizationLogFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.logs.get(organizationId, organizationLogId) -> LogsGetResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Find an organization log (only available on the scale plan and above)
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().logs().get(
    "organizationId",
    "organizationLogId",
    OrganizationLogFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**organizationLogId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations Technologies
<details><summary><code>client.organizations.technologies.list(organizationId) -> TechnologiesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().technologies().list(
    "organizationId",
    OrganizationTechnologiesListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<CatalogTechnologyFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.technologies.create(organizationId, request) -> TechnologiesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().technologies().create(
    "organizationId",
    OrganizationTechnologyCreateRequest
        .builder()
        .body(
            CatalogTechnologyRequired
                .builder()
                .color(TagColor.BLUE)
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CatalogTechnologyRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.technologies.get(organizationId, catalogTechnologyId) -> TechnologiesGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().technologies().get(
    "organizationId",
    "catalogTechnologyId",
    OrganizationTechnologyFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**catalogTechnologyId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.technologies.delete(organizationId, catalogTechnologyId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().technologies().delete(
    "organizationId",
    "catalogTechnologyId",
    OrganizationTechnologyDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**catalogTechnologyId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.technologies.update(organizationId, catalogTechnologyId, request) -> TechnologiesUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().technologies().update(
    "organizationId",
    "catalogTechnologyId",
    OrganizationTechnologyUpdateRequest
        .builder()
        .body(
            CatalogTechnologyPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**catalogTechnologyId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `CatalogTechnologyPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations Users
<details><summary><code>client.organizations.users.list(organizationId) -> UsersListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().users().list(
    "organizationId",
    OrganizationUsersListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.users.delete(organizationId, userId) -> Map&amp;lt;String, Object&amp;gt;</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().users().delete(
    "organizationId",
    "userId",
    OrganizationUserDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**userId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.users.update(organizationId, userId, request) -> UsersUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().users().update(
    "organizationId",
    "userId",
    OrganizationUserUpdateRequest
        .builder()
        .body(
            OrganizationUser
                .builder()
                .permission(PermissionType.BILLING)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**userId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `OrganizationUser` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations Logs Stats
<details><summary><code>client.organizations.logs.stats.byType(organizationId) -> OrganizationLogStatsListByType</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List total counts of actions for each action type (e.g. diagram-content-update, model-object-create)
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().logs().stats().byType(
    "organizationId",
    OrganizationLogStatsByTypeRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<OrganizationLogStatsFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**period:** `Optional<ActionLogStatsPeriod>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.logs.stats.byEntity(organizationId) -> ActionLogStatsListByEntity</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

List total counts of organizations for each entity identifier
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().logs().stats().byEntity(
    "organizationId",
    OrganizationLogStatsByEntityRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<OrganizationLogStatsFilter>` 
    
</dd>
</dl>

<dl>
<dd>

**period:** `Optional<ActionLogStatsPeriod>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Organizations Users Invites
<details><summary><code>client.organizations.users.invites.list(organizationId) -> InvitesListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().users().invites().list(
    "organizationId",
    OrganizationUserInvitesListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.users.invites.create(organizationId, request) -> InvitesCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().users().invites().create(
    "organizationId",
    OrganizationUserInviteCreateRequest
        .builder()
        .body(
            OrganizationUserInviteRequired
                .builder()
                .email("email")
                .expiresAt(OffsetDateTime.parse("2024-01-15T09:30:00Z"))
                .permission(PermissionType.BILLING)
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `OrganizationUserInviteRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.organizations.users.invites.revoke(organizationId, organizationUserInviteId) -> InvitesRevokeResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.organizations().users().invites().revoke(
    "organizationId",
    "organizationUserInviteId",
    OrganizationUserInviteRevokeRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**organizationId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**organizationUserInviteId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Tags Groups
<details><summary><code>client.tags.groups.list(landscapeId, versionId) -> GroupsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().groups().list(
    "landscapeId",
    "versionId",
    TagGroupsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**filter:** `Optional<TagGroupFilter>` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.groups.create(landscapeId, versionId, request) -> GroupsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().groups().create(
    "landscapeId",
    "versionId",
    TagGroupCreateRequest
        .builder()
        .body(
            TagGroupRequired
                .builder()
                .icon(TagGroupIcon.BUG)
                .index(1.1)
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TagGroupRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.groups.get(landscapeId, versionId, tagGroupId) -> GroupsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().groups().get(
    "landscapeId",
    "versionId",
    "tagGroupId",
    TagGroupFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagGroupId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.groups.upsert(landscapeId, versionId, tagGroupId, request) -> GroupsUpsertResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().groups().upsert(
    "landscapeId",
    "versionId",
    "tagGroupId",
    TagGroupUpsertRequest
        .builder()
        .body(
            TagGroupUpsert
                .builder()
                .icon(TagGroupIcon.BUG)
                .index(1.1)
                .name("name")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagGroupId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TagGroupUpsert` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.groups.delete(landscapeId, versionId, tagGroupId) -> GroupsDeleteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().groups().delete(
    "landscapeId",
    "versionId",
    "tagGroupId",
    TagGroupDeleteRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagGroupId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.tags.groups.update(landscapeId, versionId, tagGroupId, request) -> GroupsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.tags().groups().update(
    "landscapeId",
    "versionId",
    "tagGroupId",
    TagGroupUpdateRequest
        .builder()
        .body(
            TagGroupPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**tagGroupId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `TagGroupPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Versions Reverts
<details><summary><code>client.versions.reverts.list(landscapeId) -> RevertsListResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().reverts().list(
    "landscapeId",
    VersionRevertsListRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.reverts.create(landscapeId, request) -> RevertsCreateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().reverts().create(
    "landscapeId",
    VersionRevertCreateRequest
        .builder()
        .body(
            VersionRevertRequired
                .builder()
                .notes("notes")
                .versionId("versionId")
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `VersionRevertRequired` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.reverts.get(landscapeId, versionRevertId) -> RevertsGetResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().reverts().get(
    "landscapeId",
    "versionRevertId",
    VersionRevertFindRequest
        .builder()
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionRevertId:** `String` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.versions.reverts.update(landscapeId, versionRevertId, request) -> RevertsUpdateResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```java
client.versions().reverts().update(
    "landscapeId",
    "versionRevertId",
    VersionRevertUpdateRequest
        .builder()
        .body(
            VersionRevertPartial
                .builder()
                .build()
        )
        .build()
);
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**landscapeId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**versionRevertId:** `String` 
    
</dd>
</dl>

<dl>
<dd>

**request:** `VersionRevertPartial` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>
