---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe0cec435f438c883c647d68a725d64723f06a0c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124150"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedResource_v2 linkedResource_v2 = new LinkedResource_v2();
linkedResource_v2.webUrl = "https://microsoft.com";
linkedResource_v2.applicationName = "Microsoft";
linkedResource_v2.displayName = "Microsoft";
linkedResource_v2.externalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9";

graphClient.me().tasks().lists("AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA").linkedResources()
    .buildRequest()
    .post(linkedResource_v2);

```