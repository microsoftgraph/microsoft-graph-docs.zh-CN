---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ce68648a85c7f579af5687a3afecdda2a592def4df41b0488251fa0433a561f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookNamedItem = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Request()
    .GetAsync();

```