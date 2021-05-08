---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61365d08a3c53427120a28f35cf131b4b910908d
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240578"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberEntityType = "String";

var addMembers = new List<String>()
{
    "String"
};

var removeMembers = new List<String>()
{
    "String"
};

var addExclusions = new List<String>()
{
    "String"
};

var removeExclusions = new List<String>()
{
    "String"
};

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience
    .UpdateAudienceById(memberEntityType,addMembers,removeMembers,addExclusions,removeExclusions)
    .Request()
    .PostAsync();

```