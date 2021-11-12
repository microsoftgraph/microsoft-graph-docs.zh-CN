---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c025d9c26547b4c5582f0d17a8a82cfc1130a17b96ed5123ced36d841555d644
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"]
    .CreateLink(type,null,null,null,null)
    .Request()
    .PostAsync();

```