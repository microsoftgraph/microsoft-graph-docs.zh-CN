---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a5f72a747c4e1b92f6594ba61a9dd8c9fb5a4af84c40cf9fee80d353c52aa8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218638"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .Select("displayName,givenName,postalCode")
    .GetAsync();

```