---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ae74b6f9ef50738e28add280e3bd06d6ab91368
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Tasks.Lists
    .Delta()
    .Request()
    .GetAsync();

```