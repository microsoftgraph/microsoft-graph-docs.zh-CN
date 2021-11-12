---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54092a1f858fdda3eb3dbadf5b584a4c1f57b2d7d2e62536d362c2b171f24b96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = graphClient.print().taskDefinitions("3203656e-6069-4e10-8147-d25290b00a3c").tasks("d036638b-1272-4bba-9227-732463823ed3")
    .buildRequest()
    .get();

```