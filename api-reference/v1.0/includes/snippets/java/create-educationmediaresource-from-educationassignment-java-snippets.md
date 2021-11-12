---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eda79143f02f7b512b8fe1e17562eef6316d335
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60558727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = new EducationAssignmentResource();
educationAssignmentResource.distributeForStudentWork = false;
EducationMediaResource resource = new EducationMediaResource();
resource.displayName = "homework example.PNG";
resource.fileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF";
educationAssignmentResource.resource = resource;

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1618dfb0-3ff2-4edf-8d5c-b8f81df00e80").resources()
    .buildRequest()
    .post(educationAssignmentResource);

```