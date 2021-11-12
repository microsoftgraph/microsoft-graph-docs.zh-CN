---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e5d38e0eed4f1fad0f04a98c65262299bf722d5cd40b5c8a62d181e21c43c94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106904"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethod emailAuthenticationMethod = graphClient.me().authentication().emailMethods("3ddfcfc8-9383-446f-83cc-3ab9be4be18f")
    .buildRequest()
    .get();

```