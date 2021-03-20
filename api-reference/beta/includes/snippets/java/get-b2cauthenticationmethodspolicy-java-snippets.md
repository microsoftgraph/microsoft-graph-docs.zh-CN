---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e64d370cd2464c0935fa7879a048cbe1c4d7face
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976518"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cAuthenticationMethodsPolicy b2cAuthenticationMethodsPolicy = graphClient.policies().b2cAuthenticationMethodsPolicy()
    .buildRequest()
    .get();

```