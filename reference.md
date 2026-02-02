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
    CommentsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    CommentCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    CommentFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
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
    CommentUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
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
    CommentDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
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
    CommentUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
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
    DiagramsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DiagramCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DiagramFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramExistsRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramThumbnailsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DiagramThumbnailGetRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DomainsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DomainCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DomainFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .domainId("domainId")
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
    DomainUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .domainId("domainId")
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
    DomainDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .domainId("domainId")
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
    DomainUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .domainId("domainId")
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
    DomainExistsRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .domainId("domainId")
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
    DraftsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DraftCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DraftFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .draftId("draftId")
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
    DraftUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .draftId("draftId")
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
    DraftDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .draftId("draftId")
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
    DraftUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .draftId("draftId")
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
    DraftMergeRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .draftId("draftId")
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
    FlowsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    FlowCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    FlowFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowExistsRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowThumbnailsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    FlowThumbnailGetRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    LandscapeFindRequest
        .builder()
        .landscapeId("landscapeId")
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
    LandscapeDeleteRequest
        .builder()
        .landscapeId("landscapeId")
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
    LandscapeUpdateRequest
        .builder()
        .landscapeId("landscapeId")
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
    LandscapeDuplicateRequest
        .builder()
        .landscapeId("landscapeId")
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
    LandscapeCopyRequest
        .builder()
        .landscapeId("landscapeId")
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
    LandscapeSearchRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    OrganizationFindRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationDeleteRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationUpdateRequest
        .builder()
        .organizationId("organizationId")
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
    ShareLinkFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ShareLinkCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ShareLinkDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ShareLinkUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    TagsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    TagCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    TagFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagId("tagId")
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
    TagUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagId("tagId")
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
    TagDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagId("tagId")
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
    TagUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagId("tagId")
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
    TeamsListRequest
        .builder()
        .organizationId("organizationId")
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
    TeamCreateRequest
        .builder()
        .organizationId("organizationId")
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
    TeamFindRequest
        .builder()
        .organizationId("organizationId")
        .teamId("teamId")
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
    TeamDeleteRequest
        .builder()
        .organizationId("organizationId")
        .teamId("teamId")
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
    TeamUpdateRequest
        .builder()
        .organizationId("organizationId")
        .teamId("teamId")
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
    TeamLandscapesListRequest
        .builder()
        .organizationId("organizationId")
        .teamId("teamId")
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
    TeamModelObjectsListRequest
        .builder()
        .organizationId("organizationId")
        .teamId("teamId")
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
    VersionsListRequest
        .builder()
        .landscapeId("landscapeId")
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
    VersionCreateRequest
        .builder()
        .landscapeId("landscapeId")
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
    VersionFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    VersionDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    VersionUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    CatalogTechnologyFindRequest
        .builder()
        .catalogTechnologyId("catalogTechnologyId")
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
    CatalogTechnologySlugFindRequest
        .builder()
        .catalogTechnologySlug("catalogTechnologySlug")
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
    CommentRepliesListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
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
    CommentReplyCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
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
    CommentReplyFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
        .commentReplyId("commentReplyId")
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
    CommentReplyUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
        .commentReplyId("commentReplyId")
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
    CommentReplyDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
        .commentReplyId("commentReplyId")
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
    CommentReplyUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .commentId("commentId")
        .commentReplyId("commentReplyId")
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
    DiagramContentGenerateDescriptionRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramContentFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramContentReplaceRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramContentUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    DiagramGroupsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DiagramGroupCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    DiagramGroupFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramGroupId("diagramGroupId")
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
    DiagramGroupUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramGroupId("diagramGroupId")
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
    DiagramGroupDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramGroupId("diagramGroupId")
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
    DiagramGroupUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramGroupId("diagramGroupId")
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
    DiagramGroupExistsRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramGroupId("diagramGroupId")
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
    DiagramExportImageFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
        .diagramExportImageId("diagramExportImageId")
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
    DiagramExportImageCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .diagramId("diagramId")
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
    FlowExportTextRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowExportCodeRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    FlowExportMermaidRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .flowId("flowId")
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
    ActionLogsListRequest
        .builder()
        .landscapeId("landscapeId")
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
    ActionLogFindRequest
        .builder()
        .landscapeId("landscapeId")
        .actionLogId("actionLogId")
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
    ActionLogChildrenListRequest
        .builder()
        .landscapeId("landscapeId")
        .actionLogId("actionLogId")
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
    LandscapeExportRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    LandscapeExportFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .landscapeExportId("landscapeExportId")
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
    ActionLogStatsByTypeRequest
        .builder()
        .landscapeId("landscapeId")
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
    ActionLogStatsByEntityRequest
        .builder()
        .landscapeId("landscapeId")
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
    ModelConnectionsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ModelConnectionCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ModelConnectionFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelConnectionId("modelConnectionId")
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
    ModelConnectionUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelConnectionId("modelConnectionId")
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
    ModelConnectionDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelConnectionId("modelConnectionId")
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
    ModelConnectionUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelConnectionId("modelConnectionId")
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
    ModelConnectionGenerateDescriptionRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelConnectionId("modelConnectionId")
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
    ModelObjectsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ModelObjectCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ModelObjectFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelObjectId("modelObjectId")
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
    ModelObjectUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelObjectId("modelObjectId")
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
    ModelObjectDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelObjectId("modelObjectId")
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
    ModelObjectUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelObjectId("modelObjectId")
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
    ModelConnectionsExportCsvRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    ModelObjectDependenciesExportJsonRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .modelObjectId("modelObjectId")
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
    ModelObjectsExportCsvRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    OrganizationLandscapesListRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationLandscapeCreateRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationLogsListRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationLogFindRequest
        .builder()
        .organizationId("organizationId")
        .organizationLogId("organizationLogId")
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
    OrganizationTechnologiesListRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationTechnologyCreateRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationTechnologyFindRequest
        .builder()
        .organizationId("organizationId")
        .catalogTechnologyId("catalogTechnologyId")
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
    OrganizationTechnologyDeleteRequest
        .builder()
        .organizationId("organizationId")
        .catalogTechnologyId("catalogTechnologyId")
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
    OrganizationTechnologyUpdateRequest
        .builder()
        .organizationId("organizationId")
        .catalogTechnologyId("catalogTechnologyId")
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
    OrganizationUsersListRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationUserDeleteRequest
        .builder()
        .organizationId("organizationId")
        .userId("userId")
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
    OrganizationUserUpdateRequest
        .builder()
        .organizationId("organizationId")
        .userId("userId")
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
    OrganizationLogStatsByTypeRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationLogStatsByEntityRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationUserInvitesListRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationUserInviteCreateRequest
        .builder()
        .organizationId("organizationId")
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
    OrganizationUserInviteRevokeRequest
        .builder()
        .organizationId("organizationId")
        .organizationUserInviteId("organizationUserInviteId")
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
    TagGroupsListRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    TagGroupCreateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
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
    TagGroupFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagGroupId("tagGroupId")
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
    TagGroupUpsertRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagGroupId("tagGroupId")
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
    TagGroupDeleteRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagGroupId("tagGroupId")
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
    TagGroupUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionId("versionId")
        .tagGroupId("tagGroupId")
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
    VersionRevertsListRequest
        .builder()
        .landscapeId("landscapeId")
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
    VersionRevertCreateRequest
        .builder()
        .landscapeId("landscapeId")
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
    VersionRevertFindRequest
        .builder()
        .landscapeId("landscapeId")
        .versionRevertId("versionRevertId")
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
    VersionRevertUpdateRequest
        .builder()
        .landscapeId("landscapeId")
        .versionRevertId("versionRevertId")
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
