---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dba8882c4e3f693bee61cbdefa18b54ade90dd66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToNotebook(OnenoteSectionCopyToNotebookParameterSet
        .newBuilder()
        .withId(id)
        .withGroupId(groupId)
        .withRenameAs(renameAs)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```