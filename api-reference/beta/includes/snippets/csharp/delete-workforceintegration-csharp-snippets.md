---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfdb2afe0a1d9747817fb57e205ec4353249288c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870516"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .DeleteAsync();

```