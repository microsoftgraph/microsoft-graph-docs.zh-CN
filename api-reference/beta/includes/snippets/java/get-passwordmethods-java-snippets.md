---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fb017dbf3c33663ab6b2c08261d3f9fb380d06e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961512"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPasswordAuthenticationMethodCollectionPage passwordMethods = graphClient.me().authentication().passwordMethods()
    .buildRequest()
    .get();

```