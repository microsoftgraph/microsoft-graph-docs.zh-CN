---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cd40cb40d6181f3b1890d697c81958b90ea9312
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftApplicationDataAccessSettings = new MicrosoftApplicationDataAccessSettings
{
    DisabledForGroup = "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
};

await graphClient.Organization["{organization-id}"].Settings.MicrosoftApplicationDataAccess
    .Request()
    .UpdateAsync(microsoftApplicationDataAccessSettings);

```