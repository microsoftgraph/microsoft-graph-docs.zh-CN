---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba701f9c03d8d9cc7eaab195622b56b6cd478caf
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239688"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("{caseId}").settings()
    .resetToDefault()
    .buildRequest()
    .post();

```