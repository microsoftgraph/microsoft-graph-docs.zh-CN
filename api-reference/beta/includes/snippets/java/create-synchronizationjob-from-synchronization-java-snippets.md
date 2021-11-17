---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d0ca40c96018f8590d7b7d110197b84d9846e87f7a37119df7dc3d8fee069d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162860"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationJob synchronizationJob = new SynchronizationJob();
synchronizationJob.templateId = "BoxOutDelta";

graphClient.servicePrincipals("{id}").synchronization().jobs()
    .buildRequest()
    .post(synchronizationJob);

```