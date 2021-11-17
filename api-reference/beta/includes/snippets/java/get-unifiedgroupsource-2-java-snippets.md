---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a59877683e7328ea551fcaa5caaf65f08b68d654a38a73140ad802ae6662ed98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163437"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedGroupSource unifiedGroupSource = graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").unifiedGroupSources("33434233-3030-3739-3043-393039324633")
    .buildRequest()
    .get();

```