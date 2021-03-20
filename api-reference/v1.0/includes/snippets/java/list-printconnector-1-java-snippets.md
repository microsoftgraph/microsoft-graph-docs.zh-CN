---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f50cfd7725e4549881826dce826a10788fcd967f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948875"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintConnectorCollectionPage connectors = graphClient.print().connectors()
    .buildRequest()
    .get();

```