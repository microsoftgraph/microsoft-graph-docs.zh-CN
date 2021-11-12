---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9151a75a195822280d3e4e39bdfb88f8384ac5e52c49a6f7bf06e03159f39381
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333388"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var index = new Int32
{
};

var values = JsonDocument.Parse("[{}]");

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Columns
    .Add(index,values,null)
    .Request()
    .PostAsync();

```