---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20dd8c73743972d51237ae0d60879176abd479a0dc443b7702ed5326941edf81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Cell(5,6)
    .Request()
    .GetAsync();

```