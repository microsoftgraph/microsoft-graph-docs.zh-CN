---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6da0b4eba76825557595b27ad2e503a8bdd883fc2acd27491466fd0077775391
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Addresses["{itemAddress-id}"]
    .Request()
    .DeleteAsync();

```