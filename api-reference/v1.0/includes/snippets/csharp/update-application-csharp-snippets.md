---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca8db5cabf2ee88649dec1ed12461f1477a82ad2
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995966"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "New display name"
};

await graphClient.Applications["{id}"]
    .Request()
    .UpdateAsync(application);

```