---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ed5dc4fe7585c8ca6e09b9698ab481d29f094ea
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767101"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignmentDefaults()
    .buildRequest()
    .get();

```