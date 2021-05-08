---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7801c1c02acb3275e07d79b05b3e8ebcee86681e
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String memberEntityType = "String";

LinkedList<String> addMembersList = new LinkedList<String>();
addMembersList.add("String");

LinkedList<String> removeMembersList = new LinkedList<String>();
removeMembersList.add("String");

LinkedList<String> addExclusionsList = new LinkedList<String>();
addExclusionsList.add("String");

LinkedList<String> removeExclusionsList = new LinkedList<String>();
removeExclusionsList.add("String");

graphClient.admin().windows().updates().deployments("{deploymentId}").audience()
    .updateAudienceById(DeploymentAudienceUpdateAudienceByIdParameterSet
        .newBuilder()
        .withMemberEntityType(memberEntityType)
        .withAddMembers(addMembersList)
        .withRemoveMembers(removeMembersList)
        .withAddExclusions(addExclusionsList)
        .withRemoveExclusions(removeExclusionsList)
        .build())
    .buildRequest()
    .post();

```