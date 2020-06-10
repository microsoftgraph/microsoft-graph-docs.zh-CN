---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70a9caac0e4fc2ad69940bb82302a4ca2574c96e
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].Connectors["{id}"].MemberOf
    .Request()
    .GetAsync();

```