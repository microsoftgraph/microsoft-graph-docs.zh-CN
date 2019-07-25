---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 71592caa2fef3ff005bd2e8f868fb2f09ceeb06d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869396"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationJob synchronizationJob = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .buildRequest()
    .get();

```