---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 589b89682784a3ea867fe5e018b25c97ce1fefa8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["11021"].Assignments["19002"].Submissions["850f51b7"].Resources["f2387c3b-ec39-4bf2-a399-d7242677f024"]
    .Request()
    .DeleteAsync();

```