---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aadaf523d3a4f1fa8c67dd6ba1587a126cb5eb53
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Columns
    .Request()
    .GetAsync();

```