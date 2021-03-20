---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3eee3b78de87bba6b10211a80628253aed17d0b3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages()
    .buildRequest()
    .filter("isEnabled eq true")
    .get();

```