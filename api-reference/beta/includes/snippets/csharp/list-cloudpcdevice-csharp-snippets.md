---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b791ea808765f0e6f2bc2069df4df8cb753c5b49
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDevices = await graphClient.TenantRelationships.ManagedTenants.CloudPcDevices
    .Request()
    .GetAsync();

```