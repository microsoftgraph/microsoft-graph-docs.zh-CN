---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95dfe2b582380a85c5706e7759fa41131ecd1a66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983568"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTriggerCollectionPage taskTriggers = graphClient.print().printers("{id}").taskTriggers()
    .buildRequest()
    .get();

```