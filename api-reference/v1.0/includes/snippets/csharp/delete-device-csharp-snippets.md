---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38191c398fb4b39f5e97a7ab9754258194718267
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784371"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Devices["{device-id}"]
    .Request()
    .DeleteAsync();

```