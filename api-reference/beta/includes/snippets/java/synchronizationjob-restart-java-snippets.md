---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 970515e248844ed1b145da6d5c232a68ba0064d9a22b85fe267c5534243c1e22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903926"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer <token>"));

SynchronizationJobRestartCriteria criteria = new SynchronizationJobRestartCriteria();
criteria.resetScope = EnumSet.of(SynchronizationJobRestartScope.WATERMARK,SynchronizationJobRestartScope.ESCROWS,SynchronizationJobRestartScope.QUARANTINE_STATE);

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .restart(SynchronizationJobRestartParameterSet
        .newBuilder()
        .withCriteria(criteria)
        .build())
    .buildRequest( requestOptions )
    .post();

```