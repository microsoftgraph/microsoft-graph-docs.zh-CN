---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bed041c5b2df14931d42a9d8d3b86b8af6e40ef06d820f41f2c55d8173947ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129763"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADI4oeRpAABf0HJUAAA="]
    .Request()
    .GetAsync();

```