---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed394958afec19666cc0f424c04db1c554c10b9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].ExtensionProperties
    .Request()
    .DeleteAsync();

```