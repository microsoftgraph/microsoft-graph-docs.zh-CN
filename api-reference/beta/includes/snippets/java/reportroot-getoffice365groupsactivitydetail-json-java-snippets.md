---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bb8b249a15815cb5a967fa57a0344c4575518ba1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360455"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityDetailCollectionPage getOffice365GroupsActivityDetail = graphClient.reports()
    .getOffice365GroupsActivityDetail("D7")
    .buildRequest()
    .get();

```