---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d9ae9beb7f1a64e8523fd46179eb1ccfa3fbe8fd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872982"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageAccountDetailCollectionPage getOneDriveUsageAccountDetail = graphClient.reports()
    .getOneDriveUsageAccountDetail('D7')
    .buildRequest()
    .get();

```