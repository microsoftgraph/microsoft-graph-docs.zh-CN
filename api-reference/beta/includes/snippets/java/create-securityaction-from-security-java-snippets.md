---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a58d341f15eedc418cccf282a4809b48171bd5b0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972509"
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