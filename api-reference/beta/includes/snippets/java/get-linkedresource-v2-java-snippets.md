---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4692e55b361929636dbbd37eb1dc7d0630c1f76c
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524691"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8 = graphClient.me().tasks().lists().aAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=().tasks().aAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA().linkedResources().e2c5ed75-7aa4-4f8e-84ab-98b5e0b56ee8()
    .buildRequest()
    .get();

```