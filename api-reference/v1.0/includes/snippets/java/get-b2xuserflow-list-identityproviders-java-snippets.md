---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d893f69f9083b5f40d2a587d80eb1dfed8c5dc2
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919933"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2xUserFlows("B2X_1_Partner").identityProviders()
    .buildRequest()
    .get();

```