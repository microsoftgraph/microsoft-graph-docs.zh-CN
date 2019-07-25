---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dedcc033e3b96e945a1bd80b8a55b7c8442f8455
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886444"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("{class-id}")
    .buildRequest()
    .get();

```