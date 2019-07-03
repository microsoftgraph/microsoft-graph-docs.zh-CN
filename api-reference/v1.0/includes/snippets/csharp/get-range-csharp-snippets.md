---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f82dc5e5ef57a926ebed63c81d118f6a05e9852
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range()
    .Request()
    .GetAsync();

```