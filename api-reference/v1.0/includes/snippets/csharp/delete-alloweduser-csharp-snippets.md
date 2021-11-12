---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4bfa12fc2efbb3cccf7af5cd1e0dd41c57424c4cfba1522001f48257858f111
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Shares["{printerShare-id}"].AllowedUsers["{user-id}"].Reference
    .Request()
    .DeleteAsync();

```