---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fbc0bd549ef71d7c6a37573620a5c511340776f
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roomlist = await graphClient.Places
    .Request()
    .GetAsync();

```