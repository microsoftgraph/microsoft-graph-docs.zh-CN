---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d2fb3a9a04158367bb20d78e5d95d5e887725a711d30d310f5e8256cc6fd6dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"].Extensions["{extension-id}"]
    .Request()
    .GetAsync();

```