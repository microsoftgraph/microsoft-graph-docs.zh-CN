---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74f769a54cc5275bf2dff83959956d0321d1e70d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208889"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthIssueCollectionPage issues = graphClient.admin().serviceAnnouncement().issues()
    .buildRequest()
    .get();

```