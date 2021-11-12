---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45a23c7dacca7ded07b385f5716206fe770b1faa31f49883fdf7f4b7be896513
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278396"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Custodian custodian = new Custodian();
custodian.applyHoldToSources = false;

graphClient.compliance().ediscovery().cases("2192ca408ea2410eba3bec8ae873be6b").custodians("45454331323337443946343043464239")
    .buildRequest()
    .patch(custodian);

```