---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 525a900672e182ecf1b1e8998fcf241db381d51a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAzureADApplicationSignInSummary = await graphClient.Reports
    .GetAzureADApplicationSignInSummary('D7')
    .Request()
    .GetAsync();

```