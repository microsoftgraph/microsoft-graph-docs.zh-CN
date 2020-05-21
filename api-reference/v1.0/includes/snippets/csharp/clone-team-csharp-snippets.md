---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fd21ecbc1531a2c01c488cbe2b2d7c494b48c12
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Library Assist";

var description = "Self help community for library";

var mailNickname = "libassist";

var partsToClone = ClonableTeamParts.Apps | ClonableTeamParts.Tabs | ClonableTeamParts.Settings | ClonableTeamParts.Channels | ClonableTeamParts.Members;

var visibility = TeamVisibilityType.Public;

await graphClient.Teams["{id}"]
    .Clone(visibility,partsToClone,displayName,description,mailNickname,null)
    .Request()
    .PostAsync();

```