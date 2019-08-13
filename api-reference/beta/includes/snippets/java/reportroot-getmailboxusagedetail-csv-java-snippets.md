---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a22aad0b4aa73acd67acd221df03441553d49cf7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360559"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageDetailCollectionPage getMailboxUsageDetail = graphClient.reports()
    .getMailboxUsageDetail("D7")
    .buildRequest()
    .get();

```