---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57bfcc3b4894d47076c7b9dcf723eaab2967b345
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819889"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnotation = await graphClient.Me.Profile.Notes["{id}"]
    .Request()
    .GetAsync();

```