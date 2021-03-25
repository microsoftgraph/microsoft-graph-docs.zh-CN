---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22861b6b0b79027bdbec869a4020881f2bdcf2bc
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").defaultPages("idpselections").content()
    .buildRequest()
    .get();

```