---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f637181d096ae5c6b375b8c548ba164115c9fa8d12562debe79212deee7c9970
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333983"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean isSyncedFromOnPremises = false;

graphClient.directoryObjects()
    .getAvailableExtensionProperties(DirectoryObjectGetAvailableExtensionPropertiesParameterSet
        .newBuilder()
        .withIsSyncedFromOnPremises(isSyncedFromOnPremises)
        .build())
    .buildRequest()
    .post();

```