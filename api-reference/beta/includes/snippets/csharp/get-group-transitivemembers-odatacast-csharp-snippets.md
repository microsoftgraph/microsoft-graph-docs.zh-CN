---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f8980edfb7fd712426d627dec0432047a3ef45e5b622dcd1374302af40da932
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["{group-id}"].TransitiveMembers
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```