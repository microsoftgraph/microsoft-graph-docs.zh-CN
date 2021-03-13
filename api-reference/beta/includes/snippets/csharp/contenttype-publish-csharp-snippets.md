---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c63bea8ebae7cca0811e967086baec20daf02c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Publish()
    .Request()
    .PostAsync();

```