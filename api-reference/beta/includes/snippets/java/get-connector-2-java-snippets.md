---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bb9eeca3d9a1c96b2acd6a29e631d79ffe5e8b1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942323"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = graphClient.print().connectors("{id}")
    .buildRequest()
    .get();

```