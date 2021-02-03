---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be9a2c2fa7e7ac9f644ad70c981289f213eea225
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092530"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = graphClient.education().classes("{id}").assignmentSettings()
    .buildRequest()
    .get();

```