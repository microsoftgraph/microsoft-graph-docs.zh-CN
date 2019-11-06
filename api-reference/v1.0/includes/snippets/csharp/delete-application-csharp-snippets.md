---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39548837e8e033276140337c3ff72d35febf2db7
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"]
    .Request()
    .DeleteAsync();

```