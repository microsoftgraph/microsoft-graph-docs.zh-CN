---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f709288d10f900faae7ced4f6ee6744f44bd7794a43fc23a204426501a2bf44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Reprovision()
    .Request()
    .PostAsync();

```