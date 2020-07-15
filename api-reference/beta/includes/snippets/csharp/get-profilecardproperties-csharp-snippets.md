---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4202f7b061aed8374f1a5116cd30565757b48de8
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperties = await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties
    .Request()
    .GetAsync();

```