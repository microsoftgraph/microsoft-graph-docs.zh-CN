---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f131da6760773047ec2ce2d46171557d9aa0a95d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957241"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval["{privilegedApproval-id}"]
    .Request()
    .GetAsync();

```