---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7381c18770b61c629d5e12c309b8dbafe1f9aefe49d5188a3ef1405e6337efea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var password = "ThisIsMyPrivatePassword";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .CreateLink(type,scope,null,password,null)
    .Request()
    .PostAsync();

```