---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfb9d2fbd1af9c201070048ba054f5463dfad8c99a505dbdc21c77c59bd3a30b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcOnPremisesConnection = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections["{cloudPcOnPremisesConnection-id}"]
    .Request()
    .GetAsync();

```