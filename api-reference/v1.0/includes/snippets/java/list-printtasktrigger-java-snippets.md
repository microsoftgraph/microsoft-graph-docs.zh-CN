---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff34a3d21b7c11e6c003de4438688bd3ed420f47
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977873"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskTriggerCollectionPage taskTriggers = graphClient.print().printers("{printerId}").taskTriggers()
    .buildRequest()
    .get();

```