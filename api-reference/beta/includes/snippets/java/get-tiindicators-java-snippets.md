---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d7087476af099d218cff9a691cb90d153ef8064
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971975"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITiIndicatorCollectionPage tiIndicators = graphClient.security().tiIndicators()
    .buildRequest()
    .get();

```