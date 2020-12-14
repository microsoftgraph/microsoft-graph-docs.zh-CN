---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e1699f29bd21255179b5eb582ced2b9f42a6eb5
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658916"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Custodian custodian = new Custodian();
custodian.applyHoldToSources = false;

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians("45454331323337443946343043464239")
    .buildRequest()
    .patch(custodian);

```