---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d132425e3dffa95b42bb955b4162fb06a792def6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789123"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{device-id}"].RegisteredOwners["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```