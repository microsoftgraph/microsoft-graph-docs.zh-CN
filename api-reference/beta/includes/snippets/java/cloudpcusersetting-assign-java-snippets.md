---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85011df26f3dbd6cd69438e8d7b8944fb089e1b938708eaa86f571d81a86cdb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162098"
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