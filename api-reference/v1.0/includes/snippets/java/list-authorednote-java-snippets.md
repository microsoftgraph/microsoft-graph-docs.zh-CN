---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb0d5a50a595ff50f695fc2e83b1d7fa384cfd6f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687903"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthoredNoteCollectionPage notes = graphClient.privacy().subjectRightsRequests("{subjectRightsRequestId}").notes()
    .buildRequest()
    .get();

```