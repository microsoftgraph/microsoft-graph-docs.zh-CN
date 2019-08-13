---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94a8a17ea70af05530f87bcc36cecc1338f04218
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327395"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityUserDetail("D7")
    .buildRequest()
    .get();

```