---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b71fd0bdd2c1692f35c80901c23216cf324f021
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedLanguages = await graphClient.Me.Outlook.SupportedLanguages()
    .Request()
    .GetAsync();

```