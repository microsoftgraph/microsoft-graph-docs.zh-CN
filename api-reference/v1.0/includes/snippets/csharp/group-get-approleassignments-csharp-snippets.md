---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b53e1ba418016837f230b3bb24bee8f6e4bcee7a612d8383f3db979285106f8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignments = await graphClient.Groups["{group-id}"].AppRoleAssignments
    .Request()
    .GetAsync();

```