---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f50cfd7725e4549881826dce826a10788fcd967f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945599"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintConnectorCollectionPage connectors = graphClient.print().connectors()
    .buildRequest()
    .get();

```