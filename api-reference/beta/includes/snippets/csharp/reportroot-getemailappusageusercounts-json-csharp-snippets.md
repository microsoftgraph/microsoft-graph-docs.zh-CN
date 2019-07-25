---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4885f2298ef8580056a553b8f5c049f361864712
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserCounts = await graphClient.Reports
    .GetEmailAppUsageUserCounts('D7')
    .Request()
    .GetAsync();

```