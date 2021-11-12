---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a27840754d634a9a73354b67671a7eef45f54815c7b5bf0828211428aa23e8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218891"
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