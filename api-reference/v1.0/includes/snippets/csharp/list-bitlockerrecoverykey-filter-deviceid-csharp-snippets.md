---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdb56abbe9ae5ed64e3913b797e18799565d1d98
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730324"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recoveryKeys = await graphClient.InformationProtection.Bitlocker.RecoveryKeys
    .Request()
    .Header("ocp-client-name","\"My Friendly Client\"")
    .Header("ocp-client-version","\"1.2\"")
    .Filter("deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'")
    .GetAsync();

```