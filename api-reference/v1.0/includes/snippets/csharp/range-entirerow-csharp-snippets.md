---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf0d09662a90eb7b4cb851e501323771b8ac9843902dc0dd21cf00096f4bc523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162003"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .EntireRow()
    .Request()
    .GetAsync();

```