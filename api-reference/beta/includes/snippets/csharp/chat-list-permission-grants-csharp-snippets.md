---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f801137077504d2d397343676582bb447e75dc12f0ecad31864c06f1556ab33a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrants = await graphClient.Chats["{chat-id}"].PermissionGrants
    .Request()
    .GetAsync();

```