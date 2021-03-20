---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dd5725020d2e35317b613bca5e0cdeed2cae887
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950978"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAuthenticationMethodCollectionPage emailMethods = graphClient.me().authentication().emailMethods()
    .buildRequest()
    .get();

```