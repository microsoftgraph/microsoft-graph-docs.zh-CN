---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dc866dcbfc52de1f609aad10cda0815f5257b3f8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376067"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActiveUserDetail("D7")
    .Request()
    .GetAsync();

```