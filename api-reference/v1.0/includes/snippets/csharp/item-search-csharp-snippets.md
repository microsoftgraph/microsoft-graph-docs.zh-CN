---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e491d30b1bc48dc511c819702a41838b305baa80
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root
    .Search("Contoso Project")
    .Request()
    .GetAsync();

```