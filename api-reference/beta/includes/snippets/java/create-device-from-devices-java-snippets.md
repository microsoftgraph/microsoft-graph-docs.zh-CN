---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 723b7ee9e0d68b805fa1c1a2e873cfd55ed1ce7a77a856719f508c7bf1e63cd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218596"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = true;
LinkedList<AlternativeSecurityId> alternativeSecurityIdsList = new LinkedList<AlternativeSecurityId>();
AlternativeSecurityId alternativeSecurityIds = new AlternativeSecurityId();
alternativeSecurityIds.type = 99;
alternativeSecurityIds.identityProvider = "identityProvider-value";
alternativeSecurityIds.key = Base64.getDecoder().decode("base64Y3YxN2E1MWFlYw==");
alternativeSecurityIdsList.add(alternativeSecurityIds);
device.alternativeSecurityIds = alternativeSecurityIdsList;
device.approximateLastSignInDateTime = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");
device.deviceId = "deviceId-value";
device.deviceMetadata = "deviceMetadata-value";
device.deviceVersion = 99;

graphClient.devices()
    .buildRequest()
    .post(device);

```