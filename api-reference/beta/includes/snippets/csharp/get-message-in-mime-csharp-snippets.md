---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 243c02baf9c496c8245e613c02bdc0b0080cec3bc87ef9ff03a89784eb7b87a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Messages["{message-id}"].Content
    .Request()
    .GetAsync();

```