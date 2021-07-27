---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a94a878af011fb2cdeac5460e90ca6fcfeb3ab91
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionPage identityProviders = graphClient.identity().identityProviders()
    .buildRequest()
    .get();

```