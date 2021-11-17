---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 582e8cc0517c229988b150cfb622600a6e6b44d808eb694c3ab9162cf6ac8679
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionWithReferencesPage userFlowIdentityProviders = graphClient.identity().b2xUserFlows("B2X_1_Test").userFlowIdentityProviders()
    .buildRequest()
    .get();

```