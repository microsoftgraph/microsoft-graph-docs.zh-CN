---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c84ca773a9d9889d22e5a4d1554df5eaeeb3df28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977778"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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