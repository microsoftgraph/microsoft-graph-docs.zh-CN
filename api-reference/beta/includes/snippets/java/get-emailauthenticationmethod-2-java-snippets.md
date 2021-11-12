---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c241ffb1405f30f16f07179f11734a71ff0f9bbee5416964f2a9d83f4599f0ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163231"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethodCollectionPage emailMethods = graphClient.me().authentication().emailMethods()
    .buildRequest()
    .get();

```