---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5fee9e5a08bff224c819729e9bbcee99d76cb34
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523559"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImage cloudPcDeviceImage = new CloudPcDeviceImage();
cloudPcDeviceImage.displayName = "Display Name value";
cloudPcDeviceImage.osBuildNumber = "OS Build Number value";
cloudPcDeviceImage.operatingSystem = "Operating System value";
cloudPcDeviceImage.version = "Version value";
cloudPcDeviceImage.sourceImageResourceId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage";

graphClient.deviceManagement().virtualEndpoint().deviceImages()
    .buildRequest()
    .post(cloudPcDeviceImage);

```