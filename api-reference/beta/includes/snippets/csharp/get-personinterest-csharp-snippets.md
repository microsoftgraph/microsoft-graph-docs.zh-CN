---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25ea9be70d2528ee9552ae6f6fbbb039f205a102
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803311"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = await graphClient.Me.Profile.Interests["{personInterest-id}"]
    .Request()
    .GetAsync();

```