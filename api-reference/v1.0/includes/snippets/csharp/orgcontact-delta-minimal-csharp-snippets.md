---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e79da0abb76b07ab22b2da38b50124733300e1d
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43771150"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.Mail 
             })
    .GetAsync();

```