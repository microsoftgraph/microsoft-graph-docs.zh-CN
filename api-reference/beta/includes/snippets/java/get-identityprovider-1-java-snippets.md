---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b9c550dafe33a91a12d0fde5a9d9fdec817e3e152cf896da8dea61984dd45f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219203"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = graphClient.identityProviders("{id}")
    .buildRequest()
    .get();

```