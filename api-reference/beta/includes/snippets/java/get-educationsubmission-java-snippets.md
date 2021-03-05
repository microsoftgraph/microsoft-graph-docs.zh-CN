---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca61fdf82122ab473a9e0ef02af391400ae8733e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472995"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmission educationSubmission = graphClient.education().classes("11010").assignments("19002").submissions("33223")
    .buildRequest()
    .get();

```