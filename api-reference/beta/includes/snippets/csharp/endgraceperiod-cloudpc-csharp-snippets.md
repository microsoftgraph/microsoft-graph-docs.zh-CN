---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a27b4923e2e77b5fcd5fa36a4b527e623d93926
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59765887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .EndGracePeriod()
    .Request()
    .PostAsync();

```