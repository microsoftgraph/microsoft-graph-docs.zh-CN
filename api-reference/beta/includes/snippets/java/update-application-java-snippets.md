---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4afde5fc636666d62e9bd04b4d67d1ecd3eeb1a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983792"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.displayName = "New display name";

graphClient.applications("{id}")
    .buildRequest()
    .patch(application);

```