---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4fb3cc1fd1bf659fe587f0bd732cd19a4b76d66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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