---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9076a63f184a238ae2b45db21880ab3fcaeb6200
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionResource educationSubmissionResource = new EducationSubmissionResource();
EducationFileResource resource = new EducationFileResource();
resource.displayName = "_FTP_EDC-61424749-250820211136.pdf";
resource.fileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3";
educationSubmissionResource.resource = resource;

graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments("1618dfb0-3ff2-4edf-8d5c-b8f81df00e80").submissions("da443246-384d-673b-32db-bdba9d7f2b51").resources()
    .buildRequest()
    .post(educationSubmissionResource);

```