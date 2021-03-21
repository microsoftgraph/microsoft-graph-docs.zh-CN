---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b3f1428324de00094f6b9033c67a545f6dda355
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySetCollectionPage keySets = graphClient.trustFramework().keySets()
    .buildRequest()
    .get();

```