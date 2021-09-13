---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc2f8e96c57b9793b23ad1cc8b7376e2e0b2dd4f99ac8262c346b64af412c552
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].AppRoleAssignments["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```