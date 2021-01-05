---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44b6bc52bd4b36a33e15f96ccbc4acc731c3e3f4
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753430"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .provisionOnDemand(parametersList)
    .buildRequest()
    .post();

```