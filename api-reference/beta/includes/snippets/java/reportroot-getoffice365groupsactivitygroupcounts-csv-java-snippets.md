---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9a37b0afd46e881f861f04fa38001cd159dc4569
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360340"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityGroupCountsCollectionPage getOffice365GroupsActivityGroupCounts = graphClient.reports()
    .getOffice365GroupsActivityGroupCounts("D7")
    .buildRequest()
    .get();

```