---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09c306b492a9d7e364785bcf756db4776ca5be12c8585864a0c67f466e6cafc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333437"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = await graphClient.Sites["{site-id}"].TermStore.Groups["{termStore.group-id}"].Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .GetAsync();

```