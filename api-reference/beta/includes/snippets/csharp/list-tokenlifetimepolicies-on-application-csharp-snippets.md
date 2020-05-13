---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2ad2885ec036baab103ed1c09f120acaa81eb4f
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "41475713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicies = await graphClient.Applications["{id}"].TokenLifetimePolicies
    .Request()
    .GetAsync();

```