---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70c8e05b2ce245e301891495d67ddad24563022c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976882"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkAGUzY5QKjAAA=").attachments("AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=")
    .buildRequest()
    .get();

```