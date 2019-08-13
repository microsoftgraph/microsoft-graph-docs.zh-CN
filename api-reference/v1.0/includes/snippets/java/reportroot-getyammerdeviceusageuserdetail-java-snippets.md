---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 514cf746e8bff667b094048efa866025f0d0af6e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320260"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerDeviceUsageUserDetail("D7")
    .buildRequest()
    .get();

```