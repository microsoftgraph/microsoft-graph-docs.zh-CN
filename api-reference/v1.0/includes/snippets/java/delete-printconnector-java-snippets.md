---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5823323e88f212c5b66a5551f331c757b230c0ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772147"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().connectors("{printConnectorId}")
    .buildRequest()
    .delete();

```