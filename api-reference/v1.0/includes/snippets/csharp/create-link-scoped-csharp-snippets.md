---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67b49f32999866921afc949d6883d21a05f0d1166161385aa438182805edff63
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "edit";

var scope = "organization";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,null,null)
    .Request()
    .PostAsync();

```