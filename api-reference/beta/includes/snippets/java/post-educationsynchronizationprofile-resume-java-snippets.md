---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 971ef673e63989742c8a8cbf1830a934fac7af3e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859996"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .resume()
    .buildRequest()
    .post();

```