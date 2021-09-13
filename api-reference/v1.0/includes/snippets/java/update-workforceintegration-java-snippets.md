---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64688981d7fc84d63a17126b1c0406c9dd6a65fe26971a74e458d2581735ce15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161958"
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

graphClient.teamwork().workforceIntegrations("{workforceIntegrationId}")
    .buildRequest()
    .patch(workforceIntegration);

```