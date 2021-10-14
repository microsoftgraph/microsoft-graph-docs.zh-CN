---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80ba1d5af33b482941e97e4fc0d6d10bf9214a1b48e0e64e555c961087b63144
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Library Assist";

var description = "Self help community for library";

var mailNickname = "libassist";

var partsToClone = ClonableTeamParts.Apps | ClonableTeamParts.Tabs | ClonableTeamParts.Settings | ClonableTeamParts.Channels | ClonableTeamParts.Members;

var visibility = TeamVisibilityType.Public;

await graphClient.Teams["{team-id}"]
    .Clone(visibility,partsToClone,displayName,description,mailNickname,null)
    .Request()
    .PostAsync();

```