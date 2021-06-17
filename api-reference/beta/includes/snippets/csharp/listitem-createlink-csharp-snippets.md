---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60c221889b5a90566405b2664f067c3277f84225
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992387"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "embed";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"]
    .CreateLink(type,null,null,null,null)
    .Request()
    .PostAsync();

```