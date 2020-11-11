---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: ed1bcdc43e8ecde7e7da7098e7ded09a020fd345
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979705"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IServicePrincipalCollectionPage serviceprincipals = graphClient.serviceprincipals()
    .buildRequest()
    .get();

```