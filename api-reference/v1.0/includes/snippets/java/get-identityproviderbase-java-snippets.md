---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca42c313c1e6ff68c91b0b476d6e8975db6f4462d842518eef1a4ca4477380d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220014"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionPage identityProviders = graphClient.identity().identityProviders()
    .buildRequest()
    .get();

```