---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e759d5d52f4f2ffb4361ec98b6785c350a7d96cb6b14855f97698b0bbec69c54
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var awards = await graphClient.Me.Profile.Awards
    .Request()
    .GetAsync();

```