---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94649e031451a25545064e1eef8ec69834581e1e
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015365"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["10001"].Users["13006"]
    .Request()
    .DeleteAsync();

```