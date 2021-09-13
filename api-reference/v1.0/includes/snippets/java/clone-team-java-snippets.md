---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: def4fc061b72e846756f729e3eaecb9182f5a55367a5dbbf5cda2d9c9ac46cc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277851"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Library Assist";

String description = "Self help community for library";

String mailNickname = "libassist";

EnumSet<ClonableTeamParts> partsToClone = EnumSet.of(ClonableTeamParts.APPS,ClonableTeamParts.TABS,ClonableTeamParts.SETTINGS,ClonableTeamParts.CHANNELS,ClonableTeamParts.MEMBERS);

TeamVisibilityType visibility = TeamVisibilityType.PUBLIC;

graphClient.teams("{id}")
    .clone(TeamCloneParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withDescription(description)
        .withMailNickname(mailNickname)
        .withClassification(null)
        .withVisibility(visibility)
        .withPartsToClone(partsToClone)
        .build())
    .buildRequest()
    .post();

```