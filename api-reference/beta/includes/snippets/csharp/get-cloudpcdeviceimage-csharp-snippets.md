---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffbfb28b1a2b829d43e1e4994b18249a655bbbba97683cd965bbf589369e9046
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDeviceImage = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages["{cloudPcDeviceImage-id}"]
    .Request()
    .GetAsync();

```