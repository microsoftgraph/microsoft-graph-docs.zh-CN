---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db5bd15ecb745dd40ce6a1a90e73051d4ebf2c33
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974145"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer <token>"));

SynchronizationJobRestartCriteria criteria = new SynchronizationJobRestartCriteria();
criteria.resetScope = EnumSet.of(SynchronizationJobRestartScope.WATERMARK,SynchronizationJobRestartScope.ESCROWS,SynchronizationJobRestartScope.QUARANTINE_STATE);

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .restart(criteria)
    .buildRequest( requestOptions )
    .post();

```