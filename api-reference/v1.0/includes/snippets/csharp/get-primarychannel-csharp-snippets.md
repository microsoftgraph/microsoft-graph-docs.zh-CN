---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14b31735a8b5b61b0eeb26a5705bb2660e10a1ad
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{id}"].PrimaryChannel
    .Request()
    .GetAsync();

```