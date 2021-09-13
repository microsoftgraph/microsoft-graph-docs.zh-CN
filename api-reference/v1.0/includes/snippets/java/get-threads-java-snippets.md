---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fbb45f7b0f92be31240e83b74079f24a9d44c86
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068334"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThreadCollectionPage threads = graphClient.groups("4d81ce71-486c-41e9-afc5-e41bf2d0722a").conversations("AAQkAGRhZmRhMWM3LTYwZTktNDZmYy1hNWU1LThhZWU4NzI2YTEyZgAQABKPPJ682apIiV1UFlj7XxY=").threads()
    .buildRequest()
    .get();

```