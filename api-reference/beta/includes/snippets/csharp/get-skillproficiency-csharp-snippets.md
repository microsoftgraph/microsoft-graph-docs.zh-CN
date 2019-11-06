---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b8fcab4c8a71617ca026bb94d224729433a7c7a
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = await graphClient.Me.Profile.Skills["{id}"]
    .Request()
    .GetAsync();

```