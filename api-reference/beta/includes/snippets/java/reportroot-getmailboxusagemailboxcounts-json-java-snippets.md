---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ad896836314fd9057630de6d8a3a811a62d9a7e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873741"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageMailboxCountsCollectionPage getMailboxUsageMailboxCounts = graphClient.reports()
    .getMailboxUsageMailboxCounts('D7')
    .buildRequest()
    .get();

```