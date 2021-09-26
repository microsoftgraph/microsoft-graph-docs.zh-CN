---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46de03955ba50ca2bfe72743ed08bac1d0c677392700cc7f50a7273c7d6f4795
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{cloudPcDeviceImage-id}"]
    .Request()
    .DeleteAsync();

```