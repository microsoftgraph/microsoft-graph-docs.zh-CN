---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bc999c72cadf9ea8d682d5728f496318263210a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60995208"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SoftwareOathAuthenticationMethodCollectionPage softwareOathMethods = graphClient.me().authentication().softwareOathMethods()
    .buildRequest()
    .get();

```