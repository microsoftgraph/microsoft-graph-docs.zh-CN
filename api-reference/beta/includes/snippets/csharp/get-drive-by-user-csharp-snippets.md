---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b55affcdd14dca27051dec7bbe766a9b0cb84f9354d58ea08a260d6588a8fb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Users["{user-id}"].Drive
    .Request()
    .GetAsync();

```