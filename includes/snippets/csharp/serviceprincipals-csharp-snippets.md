---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eeff3b23a4ca5bb7294c487705ace068d54cd958
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals["b00c693f-9658-4c06-bd1b-c402c4653dea"]
    .Request()
    .Select("AppRoles")
    .GetAsync();

var appRoles = servicePrincipals.AppRoles;

```