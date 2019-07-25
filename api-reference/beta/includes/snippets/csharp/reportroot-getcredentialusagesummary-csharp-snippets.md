---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f85cb1dbfa58bfa22c868cd9cfe11378776a5072
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCredentialUsageSummary = await graphClient.Reports
    .GetCredentialUsageSummary('D30')
    .Request()
    .Filter("feature eq 'registration'")
    .GetAsync();

```