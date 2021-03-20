---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba53bdf8b74969c5baf6fcbb43096c035377c165
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971827"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = new EducationAssignmentResource();
educationAssignmentResource.distributeForStudentWork = false;

graphClient.education().classes("11021").assignments("19002").resources("850f51b7-1df9-4ec0-bd62-64a0214b9cbf")
    .buildRequest()
    .patch(educationAssignmentResource);

```