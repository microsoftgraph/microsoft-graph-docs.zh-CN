---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b989ca08847ebc97f3ee9ecdabd0e4fd11e64b29
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659508"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Custodian custodian = new Custodian();
custodian.email = "AdeleV@contoso.com";
custodian.applyHoldToSources = false;

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians()
    .buildRequest()
    .post(custodian);

```