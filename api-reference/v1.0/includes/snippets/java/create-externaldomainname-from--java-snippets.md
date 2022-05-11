---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e2f5bfbdde645a3dea45fcb7199216145490234
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314623"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalDomainName externalDomainName = new ExternalDomainName();
externalDomainName.id = "contososuites.com";

graphClient.directory().federationConfigurations("d5a56845-6845-d5a5-4568-a5d54568a5d5").microsoft.graph.samlOrWsFedExternalDomainFederation().domains()
    .buildRequest()
    .post(externalDomainName);

```