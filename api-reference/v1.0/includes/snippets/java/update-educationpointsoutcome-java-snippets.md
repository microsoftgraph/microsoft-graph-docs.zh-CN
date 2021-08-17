---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d534a7946f052a4300bf40be93a03f467581326d62373995080089c92fc5b393
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278579"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationPointsOutcome educationOutcome = new EducationPointsOutcome();
EducationAssignmentPointsGrade points = new EducationAssignmentPointsGrade();
points.points = 85.0;
educationOutcome.points = points1;

graphClient.education().classes("acdefc6b-2dc6-4e71-b1e9-6d9810ab1793").assignments("cf6005fc-9e13-44a2-a6ac-a53322006454").submissions("d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7").outcomes("9c0f2850-ff8f-4fd6-b3ac-e23077b59141")
    .buildRequest()
    .patch(educationOutcome);

```