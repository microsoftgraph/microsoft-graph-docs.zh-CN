---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b51bb60c7ca038dc8cf0e60fa26d5924508e5d19b0d43c485ad84bba6093123a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookOperation = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Operations["{workbookOperation-id}"]
    .Request()
    .GetAsync();

```