---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b9cc7f63fd2141a1296a766cbe15884fe6bb5d3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218084"
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
workforceIntegrations.supportedEntities = WorkforceIntegrationSupportedEntities.NONE;

graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .patch(workforceIntegrations);

```