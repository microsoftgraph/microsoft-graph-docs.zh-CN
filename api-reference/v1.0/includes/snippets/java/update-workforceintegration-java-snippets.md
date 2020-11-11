---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b411151d657a501eb9fc3537fd424ab549fc123
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983950"
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
workforceIntegrations.supportedEntities = EnumSet.of(WorkforceIntegrationSupportedEntities.NONE);

graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .patch(workforceIntegrations);

```