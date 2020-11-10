---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 851b6e601db3d00a5a3611bc9c386bcd6ed4f25f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969946"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemInsightsSettings itemInsightsSettings = graphClient.organization("{organizationId}").settings().itemInsights()
    .buildRequest()
    .get();

```