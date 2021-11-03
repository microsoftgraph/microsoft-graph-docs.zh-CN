---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a97935742fd250b164b100d4c7e8837aacc304886c1d5b741fae1fffd6048a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278490"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"].Columns
    .Request()
    .GetAsync();

```