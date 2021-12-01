---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd807c8e7312d77b681870d8bbb82f6997eb15940cb7f8e6ab197ae5d9067967
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278933"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = await graphClient.Me.Drive.Items["{driveItem-id}"].Permissions["{permission-id}"]
    .Request()
    .GetAsync();

```