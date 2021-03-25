---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dceb7951c4c70e88a555b8abc4e1071c50bd4ba8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209252"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").unifiedGroupSources("33434233-3030-3739-3043-393039324633")
    .buildRequest()
    .get();

```