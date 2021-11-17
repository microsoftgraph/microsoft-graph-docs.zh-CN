---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15e0f35442a36fa0c1f48abcf29b1a4965ffc204aa75e8f2c7c0c37fb5f378d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var positions = await graphClient.Me.Profile.Positions
    .Request()
    .GetAsync();

```