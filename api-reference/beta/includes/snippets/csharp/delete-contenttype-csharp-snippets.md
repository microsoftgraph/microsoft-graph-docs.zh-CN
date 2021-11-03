---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49cf5090e6d4d03afdd7a84c4e4f80216edb91dabb7bb06b1feab4ceabc6f0a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"]
    .Request()
    .DeleteAsync();

```