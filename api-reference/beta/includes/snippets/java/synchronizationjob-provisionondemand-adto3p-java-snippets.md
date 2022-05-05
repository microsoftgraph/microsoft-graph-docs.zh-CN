---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4769465a4d4e7fca30ea735fbbb45a76076d5b55
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202871"
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

graphClient.servicePrincipals("c8c95753-f628-48e1-9fab-76c2d4cf624c").synchronization().jobs("3f7565a3-fde6-4e4d-bda8-1bb70aba3612")
    .provisionOnDemand(SynchronizationJobProvisionOnDemandParameterSet
        .newBuilder()
        .withParameters(parametersList)
        .build())
    .buildRequest()
    .post();

```