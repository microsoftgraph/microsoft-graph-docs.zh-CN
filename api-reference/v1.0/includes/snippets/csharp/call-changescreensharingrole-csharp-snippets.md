---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ac9324b2249fd15644e553b51811e1b05741d97
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786424"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var role = ScreenSharingRole.Viewer;

await graphClient.Communications.Calls["{call-id}"]
    .ChangeScreenSharingRole(role)
    .Request()
    .PostAsync();

```