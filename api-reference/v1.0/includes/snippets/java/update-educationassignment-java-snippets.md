---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dedce784274950c35e30ea1104c64dbb7d22808ab0b8388b5bc2b344656d440
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105403"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignment educationAssignment = new EducationAssignment();
educationAssignment.displayName = "Week 1 reading assignment";
EducationItemBody instructions = new EducationItemBody();
instructions.contentType = BodyType.TEXT;
instructions.content = "Read chapters 1 through 3";
educationAssignment.instructions = instructions;
educationAssignment.dueDateTime = OffsetDateTimeSerializer.deserialize("2014-02-01T00:00:00Z");

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("ad8afb28-c138-4ad7-b7f5-a6986c2655a8")
    .buildRequest()
    .patch(educationAssignment);

```