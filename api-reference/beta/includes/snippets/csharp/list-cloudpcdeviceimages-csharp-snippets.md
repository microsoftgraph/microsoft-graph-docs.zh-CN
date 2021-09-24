---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa1da9ab88da182b58b607b6d65654044da6bd510e478ab9bc92ad6c372a1f0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105103"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceImages = await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages
    .Request()
    .GetAsync();

```