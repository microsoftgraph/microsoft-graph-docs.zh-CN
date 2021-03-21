---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fea2e7485f45596ea1694edf3e2ff42684e0116
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981008"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToSectionGroup(OnenoteSectionCopyToSectionGroupParameterSet
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