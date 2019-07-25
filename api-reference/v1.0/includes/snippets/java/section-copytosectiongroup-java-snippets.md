---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 761c22795daf8163e5596b12b22fd4d3faa9d563
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884079"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().sections("{id}")
    .copyToSectionGroup(id,groupId,renameAs,siteCollectionId,siteId)
    .buildRequest()
    .post();

```