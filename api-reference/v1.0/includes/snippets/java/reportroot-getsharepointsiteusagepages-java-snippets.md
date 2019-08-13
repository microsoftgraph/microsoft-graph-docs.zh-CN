---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dfb1b88429517558b9d5764cd49b96a3e4238cbd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357992"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointSiteUsagePages("D7")
    .buildRequest()
    .get();

```