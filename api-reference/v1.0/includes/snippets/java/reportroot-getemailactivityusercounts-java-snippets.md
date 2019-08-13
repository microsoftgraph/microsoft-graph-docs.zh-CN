---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 20af0aa337958b08c31af24ab5b17f92adbd8ac9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityUserCounts("D7")
    .buildRequest()
    .get();

```