---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5979281e45d0ce7d98d97e9f0d5b3d58fd0a5b8f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("assignedLicenses/any()")
    .Select("id,assignedLicenses")
    .GetAsync();

```