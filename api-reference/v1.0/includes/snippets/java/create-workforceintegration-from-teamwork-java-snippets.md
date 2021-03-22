---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c72dd5ee2049c93fca15ecb04acb48d62a8cc52
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980916"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkforceIntegration workforceIntegration = new WorkforceIntegration();
workforceIntegration.displayName = "displayName-value";
workforceIntegration.apiVersion = 99;
WorkforceIntegrationEncryption encryption = new WorkforceIntegrationEncryption();
encryption.protocol = WorkforceIntegrationEncryptionProtocol.SHARED_SECRET;
encryption.secret = "secret-value";
workforceIntegration.encryption = encryption;
workforceIntegration.isActive = true;
workforceIntegration.url = "url-value";
workforceIntegration.supportedEntities = EnumSet.of(WorkforceIntegrationSupportedEntities.NONE);

graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .post(workforceIntegration);

```