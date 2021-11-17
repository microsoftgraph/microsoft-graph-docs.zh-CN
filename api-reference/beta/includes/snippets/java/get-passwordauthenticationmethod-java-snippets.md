---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56b6b87e040588bc728a6795cdf9bcf9ff29958aa3680b8931292946028e778e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279116"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordAuthenticationMethod passwordAuthenticationMethod = graphClient.me().authentication().passwordMethods("{id}")
    .buildRequest()
    .get();

```