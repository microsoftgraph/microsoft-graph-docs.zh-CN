---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b916e42a5be3a7b47297d302f30e8aaaeaa711c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359079"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityUserCounts = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityUserCounts("D7")
    .Request()
    .GetAsync();

```