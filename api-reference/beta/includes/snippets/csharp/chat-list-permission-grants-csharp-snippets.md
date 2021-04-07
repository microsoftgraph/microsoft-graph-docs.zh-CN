---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bde669a774eeb66c8eb9096ff228881500f618f
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610694"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Chats["{chat-id}"].PermissionGrants
    .Request()
    .GetAsync();

```