---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ad1f929764ecdf056a6c40ee807d43185283d32
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774157"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Awards["{personAward-id}"]
    .Request()
    .DeleteAsync();

```