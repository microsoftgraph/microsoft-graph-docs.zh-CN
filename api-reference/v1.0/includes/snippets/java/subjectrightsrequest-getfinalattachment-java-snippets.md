---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cfb1f66e5a1bacaed6ee56506f17c5b9dd896e5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687608"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}")
    .getFinalAttachment()
    .buildRequest()
    .get();

```