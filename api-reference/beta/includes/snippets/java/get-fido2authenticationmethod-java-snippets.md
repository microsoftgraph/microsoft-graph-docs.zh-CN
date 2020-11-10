---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de65e4160809d3fd1b178ebf3ea7300b3bf30777
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954459"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IFido2AuthenticationMethodCollectionPage fido2Methods = graphClient.me().authentication().fido2Methods()
    .buildRequest()
    .get();

```