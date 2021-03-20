---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4564fc112e0a702fe47827b6665b0d84c99d4f5c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944585"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_PartnerSignUp").identityProviders("Facebook-OAUTH").reference()
    .buildRequest()
    .delete();

```