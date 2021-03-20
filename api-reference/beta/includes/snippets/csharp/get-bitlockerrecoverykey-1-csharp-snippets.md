---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0fa1ca71d6625157e75a8f514e06b90f7e367ee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944352"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recoveryKeys = await graphClient.InformationProtection.Bitlocker.RecoveryKeys
    .Request()
    .Header("ocp-client-name","\"My Friendly Client\"")
    .Header("ocp-client-version","\"1.2\"")
    .GetAsync();

```