---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdc0ccec3f23a3edc3c88b67cfbee8315f4f48aba170563319e9c8989a759a95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101328"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```