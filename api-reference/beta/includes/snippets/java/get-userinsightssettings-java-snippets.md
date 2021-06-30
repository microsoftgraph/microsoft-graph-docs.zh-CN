---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce4fbef4c54582d7bcc6b66659f5e49b177fa2b8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210342"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserInsightsSettings userInsightsSettings = graphClient.me().settings().itemInsights()
    .buildRequest()
    .get();

```