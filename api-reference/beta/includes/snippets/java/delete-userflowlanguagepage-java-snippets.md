---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53498d9d2db611bb678d193cfd389cad96d8fb92
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844910"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").overridesPages("phonefactor").content()
    .buildRequest()
    .delete();

```