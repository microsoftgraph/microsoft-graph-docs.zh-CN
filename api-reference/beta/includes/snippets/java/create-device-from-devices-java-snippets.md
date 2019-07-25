---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 13f0ffefbbd769df4e5fc2651efed3bbc8190833
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862657"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = true;
LinkedList<AlternativeSecurityId> alternativeSecurityIdsList = new LinkedList<AlternativeSecurityId>();
AlternativeSecurityId alternativeSecurityIds = new AlternativeSecurityId();
alternativeSecurityIds.type = 99;
alternativeSecurityIds.identityProvider = "identityProvider-value";
alternativeSecurityIds.key = "base64Y3YxN2E1MWFlYw==";
alternativeSecurityIdsList.add(alternativeSecurityIds);
device.alternativeSecurityIds = alternativeSecurityIdsList;
device.approximateLastSignInDateTime = "2016-10-19T10:37:00Z";
device.deviceId = "deviceId-value";
device.deviceMetadata = "deviceMetadata-value";
device.deviceVersion = 99;

graphClient.devices()
    .buildRequest()
    .post(device);

```