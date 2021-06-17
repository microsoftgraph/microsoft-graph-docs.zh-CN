---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d570353b4d9f4a4c47b8b9481fcd9fa0671aab50
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992335"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = new EducationCategory();
educationCategory.displayName = "Quizzes";

graphClient.education().classes("9a5e4047-c1dc-4243-9628-580d3c64b80c").assignmentCategories()
    .buildRequest()
    .post(educationCategory);

```