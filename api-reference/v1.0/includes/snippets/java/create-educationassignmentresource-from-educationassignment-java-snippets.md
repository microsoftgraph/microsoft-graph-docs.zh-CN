---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f789ac81360d320e35d30cd9f8d84fb1ea39a5a6bea77c0b5944965d3db1c6d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219652"
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