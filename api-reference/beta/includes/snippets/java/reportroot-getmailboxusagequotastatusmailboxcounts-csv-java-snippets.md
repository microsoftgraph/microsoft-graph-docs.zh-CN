---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d8c1c5f3331091e95b6b1d11b4142461239b515d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360585"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageQuotaStatusMailboxCountsCollectionPage getMailboxUsageQuotaStatusMailboxCounts = graphClient.reports()
    .getMailboxUsageQuotaStatusMailboxCounts("D7")
    .buildRequest()
    .get();

```