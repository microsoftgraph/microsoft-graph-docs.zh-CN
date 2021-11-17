---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d5e16a109d7bf24fac82993ab8f7c1ede69d6cef87b1b03aca33b93c18986fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var anniversaries = await graphClient.Me.Profile.Anniversaries
    .Request()
    .GetAsync();

```