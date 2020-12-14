---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b143929431227c573e7e89a352e020822b7c46f1
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659120"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").unifiedGroupSources("33434233-3030-3739-3043-393039324633")
    .buildRequest()
    .get();

```