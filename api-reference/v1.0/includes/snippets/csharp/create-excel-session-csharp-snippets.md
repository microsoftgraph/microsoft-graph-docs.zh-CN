---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7a83939a0ab5109d9dd12e264b8f26daaa76f7bfe93d9f76b2ccac7efdcfc32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var persistChanges = true;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook
    .CreateSession(persistChanges)
    .Request()
    .PostAsync();

```