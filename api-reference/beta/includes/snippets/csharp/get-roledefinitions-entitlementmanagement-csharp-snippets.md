---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82ab00f03a4743d8e3d81e9a8e56f9f1b905eda39036e7e72a9fe626e3ae1ffd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162867"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.EntitlementManagement.RoleDefinitions
    .Request()
    .GetAsync();

```