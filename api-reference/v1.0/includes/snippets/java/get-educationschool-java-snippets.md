---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3e63e2fec0bbc9fe8f8bd2ee29b7590b6e67f9d2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887740"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("{school-id}")
    .buildRequest()
    .get();

```