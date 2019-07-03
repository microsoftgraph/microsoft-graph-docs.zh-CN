---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c5ed53458a48b04fc1543c7fe146049cfe82afc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookFormatProtection = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Protection
    .Request()
    .GetAsync();

```