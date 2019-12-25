---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35ef8b014af45c52fbb4f30d3989c1a8b97fb347
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37995589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordCredential = new PasswordCredential
{
    DisplayName = "Password friendly name"
};

await graphClient.Applications["{id}"]
    .AddPassword(passwordCredential)
    .Request()
    .PostAsync();

```