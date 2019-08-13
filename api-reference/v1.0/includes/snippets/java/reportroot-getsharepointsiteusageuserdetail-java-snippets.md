---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f4d90b92a9db029d9fe2bca7b011af9119e5ee2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321797"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsageDetail("D7")
    .buildRequest()
    .get();

```