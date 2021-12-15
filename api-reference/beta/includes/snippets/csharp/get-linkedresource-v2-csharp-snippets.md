---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17952b76d2e565d98381dc26244d02cecbbc6e55
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8 = await graphClient.Me.Tasks.Lists.AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=.Tasks.AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA.LinkedResources.E2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8
    .Request()
    .GetAsync();

```