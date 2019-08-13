---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50d748b18a34fa01d6a780c9a7df764bd26e17b3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327224"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getMailboxUsageDetail("D7")
    .buildRequest()
    .get();

```