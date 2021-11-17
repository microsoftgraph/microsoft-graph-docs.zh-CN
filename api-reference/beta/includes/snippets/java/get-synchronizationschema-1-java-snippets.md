---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58611efdd866a69e30d17a47214295c0dcaebef11e68fbf148948f80f19ac6b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104698"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchema synchronizationSchema = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .buildRequest()
    .get();

```