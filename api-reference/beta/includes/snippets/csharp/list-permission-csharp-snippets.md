---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23beeb5e05604ce6416bdb07fb0cee4e53a03cca2b7afac9dacfdabbce5ec29b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106495"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Sites["{site-id}"].Permissions
    .Request()
    .GetAsync();

```