---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 114a6b2946073c2cb4d5be4954e1bac29b515007831cfe8d2a989bde757e8f7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164000"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Custodian custodian = new Custodian();
custodian.email = "AdeleV@contoso.com";
custodian.applyHoldToSources = false;

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians()
    .buildRequest()
    .post(custodian);

```