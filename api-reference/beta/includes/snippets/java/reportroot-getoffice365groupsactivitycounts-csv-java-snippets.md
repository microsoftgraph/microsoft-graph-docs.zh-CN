---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 06832ce7b2a938b2fa15ccd9ccc6615c7975a107
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308339"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityCountsCollectionPage getOffice365GroupsActivityCounts = graphClient.reports()
    .getOffice365GroupsActivityCounts("D7")
    .buildRequest()
    .get();

```