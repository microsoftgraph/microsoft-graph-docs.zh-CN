---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 048800bc87f5dbbb2bf21a7e1f4a334fae58b4c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872576"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsagePagesCollectionPage getSharePointSiteUsagePages = graphClient.reports()
    .getSharePointSiteUsagePages('D7')
    .buildRequest()
    .get();

```