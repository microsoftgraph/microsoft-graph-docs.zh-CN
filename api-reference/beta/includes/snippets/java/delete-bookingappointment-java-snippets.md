---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5ff4ed5ce56062c25e6001aadf83a4fc8e03ce16a1b750da697b2372bd9b3d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKqAAA=")
    .buildRequest()
    .delete();

```