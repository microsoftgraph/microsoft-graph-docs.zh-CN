---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 422689669f212308e3048c47509e18365cac3aaa5a425cccf9fb9c6a4348e538
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219563"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders
    .Delta()
    .Request()
    .GetAsync();

```