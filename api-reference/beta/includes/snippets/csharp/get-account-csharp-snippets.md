---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c96deaca3d25ef46ea0aa65aeef1d1b67d07f0ca287d172c1425b07abb66c29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var account = await graphClient.Me.Profile.Account
    .Request()
    .GetAsync();

```