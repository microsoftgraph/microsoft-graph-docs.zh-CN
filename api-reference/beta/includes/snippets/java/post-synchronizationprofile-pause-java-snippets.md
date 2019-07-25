---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bfe600ed97d4a5e9a6cd8539b1625b8a64cc5b68
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860052"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .pause()
    .buildRequest()
    .post();

```