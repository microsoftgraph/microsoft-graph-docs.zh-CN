---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 583bb80da1d8351a993f22f2d4784a4024eed1a0
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412126"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean isSyncedFromOnPremises = true;

graphClient.directoryObjects()
    .getAvailableExtensionProperties(DirectoryObjectGetAvailableExtensionPropertiesParameterSet
        .newBuilder()
        .withIsSyncedFromOnPremises(isSyncedFromOnPremises)
        .build())
    .buildRequest()
    .post();

```