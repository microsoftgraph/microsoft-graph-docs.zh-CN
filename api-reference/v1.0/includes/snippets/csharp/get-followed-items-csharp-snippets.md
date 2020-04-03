---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 006bd9316b777233b585673243deff7d9e292bc7
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var following = await graphClient.Me.Drive.Following
    .Request()
    .GetAsync();

```