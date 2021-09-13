---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6997c11269e60291b2fadf77fd0e6ff1559c3c010e3ca6ce03cb0dedff2d71ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var role = ScreenSharingRole.Viewer;

await graphClient.Communications.Calls["{call-id}"]
    .ChangeScreenSharingRole(role)
    .Request()
    .PostAsync();

```