---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec7039ef0ac3cff61e22d8dae8bb481818ac7da9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685066"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADhAAAW-VPeAAA="]
    .Request()
    .Select("internetMessageHeaders")
    .GetAsync();

```