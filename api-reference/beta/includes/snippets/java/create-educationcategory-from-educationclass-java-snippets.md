---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 407eac4948c8b0109f2d2d53bcc895124ef60ac80ce24ebb32c768d402860703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162913"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = new EducationCategory();
educationCategory.displayName = "Quizzes";

graphClient.education().classes("9a5e4047-c1dc-4243-9628-580d3c64b80c").assignmentCategories()
    .buildRequest()
    .post(educationCategory);

```