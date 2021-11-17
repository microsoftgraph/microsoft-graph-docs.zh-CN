---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e93ec8e78ab44333de3b6f1024f0ad5f5e625a47a76974cbdef25a9f282125c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Security.SecurityActions["{securityAction-id}"]
    .CancelSecurityAction()
    .Request()
    .PostAsync();

```