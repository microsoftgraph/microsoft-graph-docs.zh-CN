---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24fef63b26c8b01d1e7964aa457f3903fa00ffbb
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "AWS Contoso";

await graphClient.ApplicationTemplates["8b1025e4-1dd2-430b-a150-2ef79cd700f5"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```