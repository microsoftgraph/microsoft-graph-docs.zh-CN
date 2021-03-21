---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee2fb05c3162e3e9b0e0eb4db4f34a327fa37661
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955137"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").defaultPages("idpselections").content()
    .buildRequest()
    .get();

```