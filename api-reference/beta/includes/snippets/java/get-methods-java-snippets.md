---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54e315ba4a7744812ff6275a082949071ec799ac
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961517"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAuthenticationMethodCollectionPage methods = graphClient.me().authentication().methods()
    .buildRequest()
    .get();

```