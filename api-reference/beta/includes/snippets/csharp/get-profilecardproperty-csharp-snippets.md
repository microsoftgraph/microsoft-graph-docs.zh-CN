---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19e8b5a36a9fbc7e6deb8a64154516099e885da7
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties["{id}"]
    .Request()
    .GetAsync();

```