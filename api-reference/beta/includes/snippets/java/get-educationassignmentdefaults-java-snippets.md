---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69e7657fad739afdfc029c369363c9eccc2c3311
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470548"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDefaults educationAssignmentDefaults = graphClient.education().classes("{id}").assignmentDefaults()
    .buildRequest()
    .get();

```