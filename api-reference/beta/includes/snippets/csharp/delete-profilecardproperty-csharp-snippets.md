---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68bd880138f62d8d0eda94ac7188471c4ea959b8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799267"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties["{profileCardProperty-id}"]
    .Request()
    .DeleteAsync();

```