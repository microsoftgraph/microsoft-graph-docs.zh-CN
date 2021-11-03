---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 729c853328e25bc1dc0d8c163d873f4f2c2f8faf
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687800"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroup externalGroup = new ExternalGroup();
externalGroup.displayName = "Contoso Marketing";
externalGroup.description = "The product marketing team";

graphClient.external().connections("{connectionsId}").groups("{externalGroupId}")
    .buildRequest()
    .patch(externalGroup);

```