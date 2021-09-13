---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fe10783b85bc1bcaf6c853c7738eb7621f50ce2269c5bafb8eed90a0b1e4201
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notes = await graphClient.Me.Profile.Notes
    .Request()
    .GetAsync();

```