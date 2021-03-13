---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df8a9aa148e5569322991504a86e579db1ed1fb2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772119"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintConnector printConnector = graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .get();

```