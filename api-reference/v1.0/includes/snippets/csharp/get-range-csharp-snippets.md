---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd2cb10a99ee01ee5161c0d1ebc965579bf1b4aea08fb6756e56f826d83acd13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333908"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Request()
    .GetAsync();

```