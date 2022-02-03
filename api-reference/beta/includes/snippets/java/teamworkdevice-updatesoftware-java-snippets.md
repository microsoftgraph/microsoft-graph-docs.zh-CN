---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4920d57bc812b0135792c45d688ebaee419de646
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348383"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkSoftwareType softwareType = TeamworkSoftwareType.TEAMS_CLIENT;

String softwareVersion = "1.0.96.22";

graphClient.teamwork().devices("0f3ce432-e432-0f3c-32e4-3c0f32e43c0f")
    .updateSoftware(TeamworkDeviceUpdateSoftwareParameterSet
        .newBuilder()
        .withSoftwareType(softwareType)
        .withSoftwareVersion(softwareVersion)
        .build())
    .buildRequest()
    .post();

```