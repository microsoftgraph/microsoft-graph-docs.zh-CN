---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a7b3f9fc907ac7e90e3c60a8c66137d9665b5a9598cbc6bc0bd27bb776aca9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333062"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesConnections = await graphClient.DeviceManagement.VirtualEndpoint.OnPremisesConnections
    .Request()
    .GetAsync();

```