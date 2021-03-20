---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f1b9102cf9584852a1b50f951241c7c8f8ec514
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .filter("startswith(displayName,'Eric')")
    .select("displayName,signInActivity")
    .get();

```