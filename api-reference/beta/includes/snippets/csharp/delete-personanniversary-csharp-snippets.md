---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c643996767a48277a67fa6f1e4619d3a675c4cd
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Anniversaries["{id}"]
    .Request()
    .DeleteAsync();

```