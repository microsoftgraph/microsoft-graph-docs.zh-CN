---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c8bc546a98d593441603aa2c84eb03c7638a2fd8fbffabeb015886b5ac500da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162131"
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