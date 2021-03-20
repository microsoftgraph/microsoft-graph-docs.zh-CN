---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0422fc0e139790d122f638462d7bdad5775c5501
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978026"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().events("AAMkAGE1M88AADUv0uAAAG=").attachments("AAMkAGE1Mg72tgf7hJp0PICVGCc0g=")
    .buildRequest()
    .get();

```