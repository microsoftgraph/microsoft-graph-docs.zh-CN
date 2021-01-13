---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 495b2e20e78c11fa715d322557b4632d03224aa8
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsApps = await graphClient.AppCatalogs.TeamsApps
    .Request()
    .Filter("appDefinitions/any(a:a/bot ne null)")
    .Expand("appDefinitions($expand=bot)")
    .GetAsync();

```