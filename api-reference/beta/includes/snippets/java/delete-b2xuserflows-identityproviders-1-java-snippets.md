---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70d2dd24a363e8c9e7df2d4ee805a08287b9fef4
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").identityProviders("Facebook-OAUTH").reference()
    .buildRequest()
    .delete();

```