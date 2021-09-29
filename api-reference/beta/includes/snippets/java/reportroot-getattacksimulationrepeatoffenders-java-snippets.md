---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 333dd59ab93a275835879912d1f0308f351605fb
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996519"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetAttackSimulationRepeatOffendersCollectionPage getAttackSimulationRepeatOffenders = graphClient.reports()
    .getAttackSimulationRepeatOffenders()
    .buildRequest()
    .get();

```