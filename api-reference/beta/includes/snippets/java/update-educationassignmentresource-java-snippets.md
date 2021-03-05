---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 903e6365f99f02e110b5623923f431315a3a2722
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470365"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = new EducationAssignmentResource();
educationAssignmentResource.distributeForStudentWork = false;

graphClient.education().classes("11021").assignments("19002").resources("850f51b7-1df9-4ec0-bd62-64a0214b9cbf")
    .buildRequest()
    .patch(educationAssignmentResource);

```