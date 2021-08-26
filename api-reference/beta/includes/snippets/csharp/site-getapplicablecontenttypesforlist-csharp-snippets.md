---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6031f7ee5db071630a6f48a83e852200bdae8745701c01958fabb66f2024bd38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162449"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getApplicableContentTypesForList = await graphClient.Sites["{site-id}"]
    .GetApplicableContentTypesForList("listId")
    .Request()
    .GetAsync();

```