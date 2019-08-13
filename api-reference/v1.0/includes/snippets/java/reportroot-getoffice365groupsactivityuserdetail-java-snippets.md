---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f7f4e719bdd3ce50e05e858d9bf500fc1d0b04e3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326642"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityDetail("D7")
    .buildRequest()
    .get();

```