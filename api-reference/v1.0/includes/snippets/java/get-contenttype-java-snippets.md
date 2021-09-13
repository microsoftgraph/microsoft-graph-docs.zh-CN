---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc34a213340c6200ea51409a63a26a1829e77632
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147568"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentType contentType = graphClient.sites("{site-id}").contentTypes("{contentType-id}")
    .buildRequest()
    .get();

```