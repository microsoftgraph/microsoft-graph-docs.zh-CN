---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0d1475cf15cbaa1ef818ce8f93858dff9da9ef4
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919240"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].PostFederationSignup.Reference
    .Request()
    .PutAsync("{id}");

```