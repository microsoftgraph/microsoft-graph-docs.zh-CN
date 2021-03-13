---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd0d4c68ea91d900161fdf447378463a72cd43d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777129"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintSettings printSettings = new PrintSettings();
printSettings.documentConversionEnabled = true;

graphClient.customRequest("/print/settings", PrintSettings.class)
    .buildRequest()
    .patch(printSettings);

```