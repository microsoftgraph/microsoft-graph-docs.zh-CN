---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c02e01525e97e265159978eea68ce0e37a92ace
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790118"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.DeletedItems["{directoryObject-id}"]
    .Request()
    .GetAsync();

```