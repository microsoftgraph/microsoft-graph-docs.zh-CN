---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0185de53a6ad789d839343e4a6aacba18d3e915
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975823"
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