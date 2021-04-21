---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2c0a8804530af1a5d7d16b63cb3b1bfe356556f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920841"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = new IdentityUserFlowAttribute();
identityUserFlowAttribute.displayName = "Hobby";
identityUserFlowAttribute.description = "Your hobby";
identityUserFlowAttribute.dataType = IdentityUserFlowAttributeDataType.STRING;

graphClient.identity().userFlowAttributes()
    .buildRequest()
    .post(identityUserFlowAttribute);

```