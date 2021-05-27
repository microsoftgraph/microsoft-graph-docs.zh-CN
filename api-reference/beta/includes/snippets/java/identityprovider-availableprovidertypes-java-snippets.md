---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b1ac9e73ec9b29b112ad832bbb35712edd4a2a6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668767"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identity().identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```