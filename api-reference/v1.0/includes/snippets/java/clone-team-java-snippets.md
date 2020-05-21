---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7624cd1bae5ac2d7c16957bb3a735f65ba2757a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335694"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Library Assist";

String description = "Self help community for library";

String mailNickname = "libassist";

ClonableTeamParts partsToClone = ClonableTeamParts.APPS;

TeamVisibilityType visibility = TeamVisibilityType.PUBLIC;

graphClient.teams("{id}")
    .clone(displayName,description,mailNickname,null,visibility,partsToClone)
    .buildRequest()
    .post();

```