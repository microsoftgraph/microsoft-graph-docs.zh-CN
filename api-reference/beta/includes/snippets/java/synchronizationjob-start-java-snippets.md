---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45a8076222f405ffd3e26d193568231cbee6e78b2de96d335748a71bd960e4c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .start()
    .buildRequest()
    .post();

```