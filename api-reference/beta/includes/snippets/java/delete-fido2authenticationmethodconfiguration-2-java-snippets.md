---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e749951ab5635d9902f13ac186fa5545014d61237b8c74b0fa5cf485b50a773e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333703"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("TemporaryAccessPass")
    .buildRequest()
    .delete();

```