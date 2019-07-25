---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd2159512a5534b8084559c71f8d31b85ddb058f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872533"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteUsageStorageCollectionPage getSharePointSiteUsageStorage = graphClient.reports()
    .getSharePointSiteUsageStorage('D7')
    .buildRequest()
    .get();

```