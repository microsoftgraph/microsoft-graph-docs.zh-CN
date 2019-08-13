---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ad069885f0a23a57f1255c6831e6207d4988f880
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityDetail("D7")
    .Request()
    .GetAsync();

```