---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9da3057f399e238660498b491ff63273ac89c5c0033782833937911f7e2e88ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Oauth2PermissionGrants
    .Delta()
    .Request()
    .GetAsync();

```