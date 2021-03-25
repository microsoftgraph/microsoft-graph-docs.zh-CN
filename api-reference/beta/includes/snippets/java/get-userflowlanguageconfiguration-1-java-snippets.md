---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b15ac02eb42b9645921b131d9508028aacb3276
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210687"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages()
    .buildRequest()
    .get();

```