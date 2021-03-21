---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec5a5c5225451db79627cdd80c178a569add16d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969636"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().taskDefinitions("{printTaskDefinitionId}")
    .buildRequest()
    .delete();

```