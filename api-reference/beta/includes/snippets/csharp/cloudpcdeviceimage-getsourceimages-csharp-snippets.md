---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ec3aee50ce1634522740aa682c2c0ed1c997b630cc7cdb4000d8f634dcbde6b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSourceImages = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages
    .GetSourceImages()
    .Request()
    .GetAsync();

```