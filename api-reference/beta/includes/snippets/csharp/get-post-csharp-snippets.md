---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 989c2215e01dad640f0f5e615117a0f274ed21bee18d1243d374fbc85fced749
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"]
    .Request()
    .GetAsync();

```