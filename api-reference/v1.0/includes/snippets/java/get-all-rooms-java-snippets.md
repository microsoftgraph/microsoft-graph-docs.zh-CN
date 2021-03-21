---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c5f4982a1cda719179853d87891ba9f111ad027
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982361"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomCollectionPage room = graphClient.places().microsoft.graph.room()
    .buildRequest()
    .get();

```