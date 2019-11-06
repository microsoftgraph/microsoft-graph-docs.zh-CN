---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f934ee898628f49e095b4e706ba2d02fbecb6c1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = await graphClient.Me.Profile.EducationalActivities["{id}"]
    .Request()
    .GetAsync();

```