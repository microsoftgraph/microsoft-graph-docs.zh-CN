---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bcfd3bb9411484533d2d8d7a63a3bd48c1e96ca
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984222"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = false;
LinkedList<AlternativeSecurityId> alternativeSecurityIdsList = new LinkedList<AlternativeSecurityId>();
AlternativeSecurityId alternativeSecurityIds = new AlternativeSecurityId();
alternativeSecurityIds.type = 2;
alternativeSecurityIds.key = Base64.getDecoder().decode("base64Y3YxN2E1MWFlYw==");
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