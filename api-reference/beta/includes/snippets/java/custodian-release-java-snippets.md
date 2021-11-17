---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a16bfafc0f9e0a5d2bf6e95dec00d861c8cbee86f48ce6700066251b5399f4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163823"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians("45454331323337443946343043464239")
    .release()
    .buildRequest()
    .post();

```