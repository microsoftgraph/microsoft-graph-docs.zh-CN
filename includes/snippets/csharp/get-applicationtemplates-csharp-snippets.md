---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89fdf13c0347789cdf856eae7228aa2a17c0acfc
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplates = await graphClient.ApplicationTemplates
    .Request()
    .GetAsync();

```