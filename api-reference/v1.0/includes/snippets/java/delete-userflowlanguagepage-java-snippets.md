---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cf4653436f0c6c1fd4f1875c1bbdc7144f8e08d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666607"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en").overridesPages("selfasserted1_1").content()
    .buildRequest()
    .delete();

```