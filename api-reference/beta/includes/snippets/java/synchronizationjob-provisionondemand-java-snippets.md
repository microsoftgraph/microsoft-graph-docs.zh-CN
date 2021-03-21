---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5da6b90a11bd1d569e72a7318c0da941a09c4f06
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979381"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SynchronizationJobApplicationParameters> parametersList = new LinkedList<SynchronizationJobApplicationParameters>();
SynchronizationJobApplicationParameters parameters = new SynchronizationJobApplicationParameters();
LinkedList<SynchronizationJobSubject> subjectsList = new LinkedList<SynchronizationJobSubject>();
SynchronizationJobSubject subjects = new SynchronizationJobSubject();
subjects.objectId = "9bb0f679-a883-4a6f-8260-35b491b8b8c8";
subjects.objectTypeName = "User";
subjectsList.add(subjects);
parameters.subjects = subjectsList;
parameters.ruleId = "ea807875-5618-4f0a-9125-0b46a05298ca";

parametersList.add(parameters);

graphClient.servicePrincipals("{servicePrincipalsId}").synchronization().jobs("{synchronizationJobId}")
    .provisionOnDemand(SynchronizationJobProvisionOnDemandParameterSet
        .newBuilder()
        .withParameters(parametersList)
        .build())
    .buildRequest()
    .post();

```