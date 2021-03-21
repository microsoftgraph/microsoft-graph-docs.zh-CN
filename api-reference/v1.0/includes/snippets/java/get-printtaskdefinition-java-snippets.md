---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da2f2339bd0ab4803685e36c2f8399cd0484ad7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978688"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = graphClient.print().taskDefinitions("{printTaskDefinitionId}")
    .buildRequest()
    .get();

```