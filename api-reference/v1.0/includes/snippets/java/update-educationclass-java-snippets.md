---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aa2423d966e97e9f53ecc530e133802569a8ab9f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881495"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = new EducationClass();
educationClass.description = "History - World History 1";
educationClass.displayName = "World History Level 1";

graphClient.education().classes("{class-id}")
    .buildRequest()
    .patch(educationClass);

```