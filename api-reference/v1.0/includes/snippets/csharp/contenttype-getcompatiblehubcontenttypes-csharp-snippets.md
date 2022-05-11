---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f14661e3975617002361abc2007e7116d9944f9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316099"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCompatibleHubContentTypes = await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .GetCompatibleHubContentTypes()
    .Request()
    .GetAsync();

```