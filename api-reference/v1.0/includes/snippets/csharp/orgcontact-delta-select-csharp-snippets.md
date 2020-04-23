---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d280c12cec79a683c332846c817f1698d7bafc1
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.Mail 
             })
    .GetAsync();

```