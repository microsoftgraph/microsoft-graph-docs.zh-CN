---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83f3129bff6bc95cd655aa8971ffd28206d9d03a
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content 51d8a471-2e9d-4f53-9937-c33a8742d28f = graphClient.me().tasks().lists().aAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=().tasks().aAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA().checklistitems().51d8a471-2e9d-4f53-9937-c33a8742d28f()
    .buildRequest()
    .get();

```