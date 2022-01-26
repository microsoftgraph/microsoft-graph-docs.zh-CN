---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f14661e3975617002361abc2007e7116d9944f9
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225245"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCompatibleHubContentTypes = await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .GetCompatibleHubContentTypes()
    .Request()
    .GetAsync();

```