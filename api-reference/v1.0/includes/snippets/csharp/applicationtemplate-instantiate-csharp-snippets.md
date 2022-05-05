---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 878ee0f35876c7a0c50c9b6469100919ae334535
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220326"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Azure AD SAML Toolkit";

await graphClient.ApplicationTemplates["{applicationTemplate-id}"]
    .Instantiate(displayName)
    .Request()
    .PostAsync();

```