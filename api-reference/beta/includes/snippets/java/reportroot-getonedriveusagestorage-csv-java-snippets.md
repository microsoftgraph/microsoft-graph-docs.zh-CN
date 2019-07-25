---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9ba394c5d0b4951a0e8d100ee3860f9f4c848a47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872911"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteUsageStorageCollectionPage getOneDriveUsageStorage = graphClient.reports()
    .getOneDriveUsageStorage('D7')
    .buildRequest()
    .get();

```