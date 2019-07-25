---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3707cda6d3378f7a8db9f3367349bf3a0c7d8fe3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856036"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.accessReviews("2975E9B5-44CE-4E71-93D3-30F03B5AA992")
    .resetDecisions()
    .buildRequest()
    .post();

```