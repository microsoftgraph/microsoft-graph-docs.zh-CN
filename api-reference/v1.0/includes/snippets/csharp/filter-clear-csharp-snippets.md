---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dc76a3f9452571f9e28eed9d0be26fecbb0419d
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35740261"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"].Filter
    .Clear()
    .Request()
    .PostAsync();

```