---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 630d3cea712452123f1d23a8a2102a87005d237f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recoveryKeys = await graphClient.Bitlocker.RecoveryKeys
    .Request()
    .Header("ocp-client-name","\"My Friendly Client\"")
    .Header("ocp-client-version","\"1.2\"")
    .Filter("deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'")
    .GetAsync();

```