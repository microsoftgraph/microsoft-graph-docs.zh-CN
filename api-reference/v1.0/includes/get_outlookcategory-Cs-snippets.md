---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 68db4a30fc67c100faf93fdc5d6619f1575e1991
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookCategory = await graphClient.Me.Outlook.MasterCategories["de912e4d-c790-4da9-949c-ccd933aaa0f7"]
    .Request()
    .GetAsync();

```