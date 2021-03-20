---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3579e6a3f076b7d9cecf962d9114849791aaa1a3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967775"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroupCollectionPage audioRoutingGroups = graphClient.communications().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .get();

```