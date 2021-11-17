---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 998386b0e2e9f27993cb18f0ea9b36dd9953e110b0d90efa78b5397affb8506e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"]
    .Request()
    .GetAsync();

```