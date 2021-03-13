---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 790d93bc48bd9c720b680d8bfb42beab65895e0f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768653"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintTaskCollectionPage tasks = graphClient.print().taskDefinitions("{taskDefinitionId}").tasks()
    .buildRequest()
    .get();

```