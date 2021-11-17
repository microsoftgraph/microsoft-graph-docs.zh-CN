---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2daaf22542d2d2eaffa4d8c303ed066cd0c2261f04810140c49f8f6e7e9f7d4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219448"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDevice = await graphClient.TenantRelationships.ManagedTenants.CloudPcDevices["{managedTenants.cloudPcDevice-id}"]
    .Request()
    .GetAsync();

```