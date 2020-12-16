---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bf180212c07085a25392b1557d751d1673410b4
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692585"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Case _case = new Case();
_case.displayName = "My Case 1";

graphClient.compliance().ediscovery().cases()
    .buildRequest()
    .post(_case);

```