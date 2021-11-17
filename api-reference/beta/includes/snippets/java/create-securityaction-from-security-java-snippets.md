---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6cc5160bfac73bb6932974d49b5e4dbc81a06b7418d9b90bf6c84c8691925ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104481"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecurityAction securityAction = new SecurityAction();
securityAction.name = "BlockIp";
securityAction.actionReason = "Test";
LinkedList<KeyValuePair> parametersList = new LinkedList<KeyValuePair>();
KeyValuePair parameters = new KeyValuePair();
parameters.name = "IP";
parameters.value = "1.2.3.4";
parametersList.add(parameters);
securityAction.parameters = parametersList;
SecurityVendorInformation vendorInformation = new SecurityVendorInformation();
vendorInformation.provider = "Windows Defender ATP";
vendorInformation.vendor = "Microsoft";
securityAction.vendorInformation = vendorInformation;

graphClient.security().securityActions()
    .buildRequest()
    .post(securityAction);

```