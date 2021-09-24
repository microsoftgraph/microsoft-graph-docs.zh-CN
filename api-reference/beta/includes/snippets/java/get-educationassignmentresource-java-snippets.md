---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e88a6fb47d34189436c63179563b90fc67475a2
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508405"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResource educationAssignmentResource = graphClient.education().classes("f4a941ff-9da6-4707-ba5b-0eae93cad0b4").assignments("9018ae7a-9953-4796-a152-4c54e0910922").resources("eec7f642-9d9a-406f-bbae-4b3b2c12e273")
    .buildRequest()
    .get();

```