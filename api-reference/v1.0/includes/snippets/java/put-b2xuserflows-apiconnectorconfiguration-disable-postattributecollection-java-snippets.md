---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55e28097132701db056ddbf0146f643c803caf9b
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868841"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();

graphClient.identity().b2xUserFlows("B2X_1_testuserflow").postAttributeCollection().reference()
    .buildRequest()
    .put(identityApiConnector);

```