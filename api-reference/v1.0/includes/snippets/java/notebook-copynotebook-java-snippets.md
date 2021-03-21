---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e7cb10e540c304087bd7b881d4ded3f8eb7246e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977865"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().notebooks("{id}")
    .copyNotebook(NotebookCopyNotebookParameterSet
        .newBuilder()
        .withGroupId(groupId)
        .withRenameAs(renameAs)
        .withNotebookFolder(null)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```