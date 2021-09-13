---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7820e7108922b2bb6a964310b7cf1ff90bf73cc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean _boolean = graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .isPublished()
    .buildRequest()
    .get();

```