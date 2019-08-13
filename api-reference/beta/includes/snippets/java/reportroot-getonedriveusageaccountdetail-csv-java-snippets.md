---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b48f88e03392b94db368ab729e242b0de9a4343d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360006"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageAccountDetailCollectionPage getOneDriveUsageAccountDetail = graphClient.reports()
    .getOneDriveUsageAccountDetail("D7")
    .buildRequest()
    .get();

```