---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dbe9fd97c997b4b8e7ad119183c46db1057d0b46
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859981"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .start()
    .buildRequest()
    .post();

```