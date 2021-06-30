---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a810ee64e15672651a86affbeeaf8cbbf53042a9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207111"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<CloudPcUserSettingAssignment> assignmentsList = new LinkedList<CloudPcUserSettingAssignment>();
CloudPcUserSettingAssignment assignments = new CloudPcUserSettingAssignment();
assignments.id = "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff";
CloudPcManagementGroupAssignmentTarget target = new CloudPcManagementGroupAssignmentTarget();
target.groupId = "64ff06de-9c00-4a5a-98b5-7f5abe26ffff";
assignments.target = target;

assignmentsList.add(assignments);
CloudPcUserSettingAssignmentCollectionResponse cloudPcUserSettingAssignmentCollectionResponse = new CloudPcUserSettingAssignmentCollectionResponse();
cloudPcUserSettingAssignmentCollectionResponse.value = assignmentsList;
CloudPcUserSettingAssignmentCollectionPage cloudPcUserSettingAssignmentCollectionPage = new CloudPcUserSettingAssignmentCollectionPage(cloudPcUserSettingAssignmentCollectionResponse, null);

graphClient.deviceManagement().virtualEndpoint().userSettings("b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff")
    .assign(CloudPcUserSettingAssignParameterSet
        .newBuilder()
        .withAssignments(assignmentsList)
        .build())
    .buildRequest()
    .post();

```