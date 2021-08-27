---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b91e6d7c9ab3e8145c45aac28753898737cc6813daec5a960399e84da6c83f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409530"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identity().identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```