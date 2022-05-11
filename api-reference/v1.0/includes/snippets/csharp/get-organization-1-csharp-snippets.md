---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 520d81ba6fa155b01e6efe43dfb92b17bb89561b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization["{organization-id}"]
    .Request()
    .GetAsync();

```