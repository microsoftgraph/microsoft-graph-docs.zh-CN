---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 33a413ebb204290e7dab462804b2443e6f5e3feb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321795"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityUserDetail("D7")
    .buildRequest()
    .get();

```