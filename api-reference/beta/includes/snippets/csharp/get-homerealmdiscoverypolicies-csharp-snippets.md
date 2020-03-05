---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35cf1d0c6eedbc75c06f7a410669898877e36787
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var policy = await graphClient.Policies["homeRealmDiscoveryPolicies"]
    .Request()
    .GetAsync();

```