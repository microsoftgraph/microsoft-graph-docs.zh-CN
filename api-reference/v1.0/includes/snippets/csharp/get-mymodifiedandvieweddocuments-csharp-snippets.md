---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88496399eebde620b3e65af44867ae81082a225dd95aa32f16b02594f5afcf9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var used = await graphClient.Me.Insights.Used
    .Request()
    .OrderBy("LastUsed/LastAccessedDateTime desc")
    .GetAsync();

```