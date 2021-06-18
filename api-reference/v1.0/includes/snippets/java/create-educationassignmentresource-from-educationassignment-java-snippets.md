---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a23f5c50148c203074df744df2cbe564531de37a
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = new EducationAssignmentResource();
educationAssignmentResource.distributeForStudentWork = false;
EducationLinkResource resource = new EducationLinkResource();
resource.displayName = "Bing";
resource.link = "https://www.bing.com";
educationAssignmentResource.resource = resource;

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8").resources()
    .buildRequest()
    .post(educationAssignmentResource);

```