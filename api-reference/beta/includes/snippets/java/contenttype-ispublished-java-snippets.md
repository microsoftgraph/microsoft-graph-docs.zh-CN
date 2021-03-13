---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ded9a026f42b20191509cf5bfd7b0e8247ed698
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770572"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean _boolean = graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .isPublished()
    .buildRequest()
    .get();

```