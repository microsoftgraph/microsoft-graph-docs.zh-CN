---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 187b208ac240947df0b17165815873eca3a18f51
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "Display name"
};

await graphClient.Applications
    .Request()
    .AddAsync(application);

```