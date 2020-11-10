---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf298b79e13738ba28325e82a62db9041a552d20
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961448"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPhoneAuthenticationMethodCollectionPage phoneMethods = graphClient.me().authentication().phoneMethods()
    .buildRequest()
    .get();

```