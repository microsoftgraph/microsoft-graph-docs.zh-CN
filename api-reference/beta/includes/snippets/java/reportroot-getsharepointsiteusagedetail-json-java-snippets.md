---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dfb940a7641302ca97623750282d81afb690fe38
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359658"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsageDetailCollectionPage getSharePointSiteUsageDetail = graphClient.reports()
    .getSharePointSiteUsageDetail("D7")
    .buildRequest()
    .get();

```