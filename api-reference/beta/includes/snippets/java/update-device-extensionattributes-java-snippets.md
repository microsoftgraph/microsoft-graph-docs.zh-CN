---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20e9f09fd457a12238e7bd63530c7adab460ff24
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719265"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
OnPremisesExtensionAttributes extensionAttributes = new OnPremisesExtensionAttributes();
extensionAttributes.extensionAttribute1 = "BYOD-Device";
device.extensionAttributes = extensionAttributes;

graphClient.devices("7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac")
    .buildRequest()
    .patch(device);

```