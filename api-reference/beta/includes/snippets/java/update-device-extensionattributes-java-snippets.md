---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bed66164022a3ce4b4f3cc34cfc8d68ad594d053
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688580"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
OnPremisesExtensionAttributes extensionAttributes = new OnPremisesExtensionAttributes();
extensionAttributes.extensionAttribute1 = "BYOD-Device";
device.extensionAttributes = extensionAttributes;

graphClient.devices("{id}")
    .buildRequest()
    .patch(device);

```