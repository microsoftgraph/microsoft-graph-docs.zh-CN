---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11971f5b680121884faf949498d56f9c1f6d37c0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350504"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IServicePrincipalCollectionPage servicePrincipals = graphClient.servicePrincipals()
    .buildRequest()
    .get();

```