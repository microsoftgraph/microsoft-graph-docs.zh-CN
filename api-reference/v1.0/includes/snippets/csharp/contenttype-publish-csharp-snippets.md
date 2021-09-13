---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c63bea8ebae7cca0811e967086baec20daf02c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038268"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Publish()
    .Request()
    .PostAsync();

```