---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f65531bc927dff1b27aa2a2284d697445fb45464
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999077"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```