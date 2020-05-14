---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51a768ea7d6e183256fe74e110dc8f3b1f6d6efd
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teamwork.WorkforceIntegrations["{workforceIntegrationId}"]
    .Request()
    .DeleteAsync();

```