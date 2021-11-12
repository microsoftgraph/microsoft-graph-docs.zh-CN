---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1ca6556618cc936add3dd27d8697e0c6c32aca9ceb511a176d1909084e01734
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218821"
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