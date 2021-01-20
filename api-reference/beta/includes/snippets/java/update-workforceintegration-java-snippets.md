---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b68bc875368448e1d1a74cd098ab2921410adee1
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910610"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegration workforceIntegration = new WorkforceIntegration();
workforceIntegration.displayName = "displayName-value";
workforceIntegration.apiVersion = 99;
WorkforceIntegrationEncryption encryption = new WorkforceIntegrationEncryption();
encryption.protocol = WorkforceIntegrationEncryptionProtocol.SHARED_SECRET;
encryption.secret = "secret-value";
workforceIntegration.encryption = encryption;
workforceIntegration.isActive = true;
workforceIntegration.url = "url-value";
workforceIntegration.supports = EnumSet.of(WorkforceIntegrationSupportedEntities.NONE);

graphClient.teamwork().workforceIntegrations("{workforceIntegrationId}")
    .buildRequest()
    .patch(workforceIntegration);

```