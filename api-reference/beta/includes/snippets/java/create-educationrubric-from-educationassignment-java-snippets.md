---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46cb6a231d32a4cae8da2644a3c067a8815f01aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966500"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = new EducationRubric();
educationRubric.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"));

graphClient.education().classes("{id}").assignments("{id}").rubric().reference()
    .buildRequest()
    .put(educationRubric);

```