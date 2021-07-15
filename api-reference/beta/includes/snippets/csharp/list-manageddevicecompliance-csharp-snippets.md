---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c956159da5b4e39327c595f9a02ad6a0867211
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442019"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceCompliances = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceCompliances
    .Request()
    .GetAsync();

```