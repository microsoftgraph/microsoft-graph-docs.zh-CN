---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a113196f7e6f22c8bd3722a977bf30c005a178744194c04552f8ac02960293a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Sites["{site-id}"].Drive
    .Request()
    .GetAsync();

```