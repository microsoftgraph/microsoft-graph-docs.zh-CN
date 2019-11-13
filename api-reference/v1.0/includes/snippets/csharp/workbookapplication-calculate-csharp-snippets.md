---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69762d057c18edc282cd217fca59d9610362d806
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calculationType = "calculationType-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Application
    .Calculate(calculationType)
    .Request()
    .PostAsync();

```