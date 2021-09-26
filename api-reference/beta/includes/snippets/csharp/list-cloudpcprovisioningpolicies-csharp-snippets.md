---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 648c0258afa25277606d93e94293d7bc3ce99d36b33a4e8de1db6c9228c3a71f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var provisioningPolicies = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies
    .Request()
    .GetAsync();

```