---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1208a2ef112a943f25001c328bd00a02e87b4ea
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41493494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Drive.Items["{id}"].Workbook.Comments["{id}"].Replies
    .Request()
    .GetAsync();

```