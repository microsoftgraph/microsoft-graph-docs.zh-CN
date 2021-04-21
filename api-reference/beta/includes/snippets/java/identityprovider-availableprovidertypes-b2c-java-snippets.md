---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b1ac9e73ec9b29b112ad832bbb35712edd4a2a6
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identity().identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```