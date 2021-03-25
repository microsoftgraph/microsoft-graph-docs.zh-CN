---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d082fadb8781b908dff1b3b869da4a2e365fb5d9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208937"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionPage identityProviders = graphClient.identityProviders()
    .buildRequest()
    .get();

```