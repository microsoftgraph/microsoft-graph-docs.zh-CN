---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f2c7e08696ff76f405bf120d680e4115526dcd267c29b70fc257645eee368f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].RejectedSenders.References
    .Request()
    .DeleteAsync();

```