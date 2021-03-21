---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83ae53bbbb66e5da49ecd47d161513cf61eba8a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967221"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainCollectionPage domains = graphClient.domains()
    .buildRequest()
    .get();

```