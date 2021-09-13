---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55d3b3f83ab0b552d0ce1b77f42bcb99d231b32cf8f06ae4e75e1f05af90c551
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277574"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2xUserFlows("B2X_1_Partner").identityProviders()
    .buildRequest()
    .get();

```