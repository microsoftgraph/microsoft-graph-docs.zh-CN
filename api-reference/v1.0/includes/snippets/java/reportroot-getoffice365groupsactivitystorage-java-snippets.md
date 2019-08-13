---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b73e33c83e098d7b3617e41e8164c266238f5789
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373609"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityStorage("D7")
    .buildRequest()
    .get();

```