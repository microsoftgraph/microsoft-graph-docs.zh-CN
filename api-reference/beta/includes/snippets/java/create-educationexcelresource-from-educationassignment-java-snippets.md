---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68a4b8e578438ac53e6f562e1eba29216eb8455a
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60559450"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = new EducationAssignmentResource();
educationAssignmentResource.distributeForStudentWork = false;
EducationExcelResource resource = new EducationExcelResource();
resource.displayName = "Graph Doc pages.xlsx";
resource.fileUrl = "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2";
educationAssignmentResource.resource = resource;

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1618dfb0-3ff2-4edf-8d5c-b8f81df00e80").resources()
    .buildRequest()
    .post(educationAssignmentResource);

```