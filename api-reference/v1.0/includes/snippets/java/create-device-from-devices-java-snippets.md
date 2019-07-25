---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c2e664a49d44ae1550efbe5998775f9bf2110d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883358"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = false;
LinkedList<AlternativeSecurityId> alternativeSecurityIdsList = new LinkedList<AlternativeSecurityId>();
AlternativeSecurityId alternativeSecurityIds = new AlternativeSecurityId();
alternativeSecurityIds.type = 2;
alternativeSecurityIds.key = "base64Y3YxN2E1MWFlYw==";
alternativeSecurityIdsList.add(alternativeSecurityIds);
device.alternativeSecurityIds = alternativeSecurityIdsList;
device.deviceId = "4c299165-6e8f-4b45-a5ba-c5d250a707ff";
device.displayName = "Test device";
device.operatingSystem = "linux";
device.operatingSystemVersion = "1";

graphClient.devices()
    .buildRequest()
    .post(device);

```