---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e47009a1b8bfdf2c5e13b591fc66da01383124d2cfdd3352c467e41ee3e06ecb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274201"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPC = await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs["{cloudPC-id}"]
    .Request()
    .GetAsync();

```