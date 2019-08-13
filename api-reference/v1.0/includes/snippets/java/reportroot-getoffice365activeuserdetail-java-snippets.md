---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64aaafb0d200c3d7211e1325e2dbec814476f129
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376066"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActiveUserDetail("D7")
    .buildRequest()
    .get();

```