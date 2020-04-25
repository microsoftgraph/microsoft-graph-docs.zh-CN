---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41447be03cfb16602373ef199db72493f02e2d37
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].TokenIssuancePolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```