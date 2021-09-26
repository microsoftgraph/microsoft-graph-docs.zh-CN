---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 779c17bd2f0e2486496d273bac5a8b61172b9619
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766205"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignmentSettings()
    .buildRequest()
    .get();

```