---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e534819d41e046901ecacd41ab269338193f7c2a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887566"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = graphClient.education().users("{user-id}")
    .buildRequest()
    .get();

```