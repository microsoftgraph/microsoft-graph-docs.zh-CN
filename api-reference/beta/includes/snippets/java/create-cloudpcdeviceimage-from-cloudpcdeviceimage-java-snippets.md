---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50787756802a3c0cbcc8c78aad42bcdad0b58acf08c37b0a9d52c160a1698554
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221288"
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