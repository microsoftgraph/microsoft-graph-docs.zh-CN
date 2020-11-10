---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b24e493cb3f41f68a7867355cedc355ff567199
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970541"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegration workforceIntegrations = new WorkforceIntegration();
workforceIntegrations.displayName = "displayName-value";
workforceIntegrations.apiVersion = 99;
WorkforceIntegrationEncryption encryption = new WorkforceIntegrationEncryption();
encryption.protocol = WorkforceIntegrationEncryptionProtocol.SHARED_SECRET;
encryption.secret = "secret-value";
workforceIntegrations.encryption = encryption;
workforceIntegrations.isActive = true;
workforceIntegrations.url = "url-value";
workforceIntegrations.supports = EnumSet.of(WorkforceIntegrationSupportedEntities.NONE);

graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .patch(workforceIntegrations);

```