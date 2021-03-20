---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b0f5b3aaa6b8243ae1723f26c482c0cb06f625e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944788"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages()
    .buildRequest()
    .get();

```