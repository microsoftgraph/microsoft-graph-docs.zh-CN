---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f4d591938abab6e1da525f1131eb37d4dd0f93c
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142539"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties.Fax
    .Request()
    .DeleteAsync();

```