---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 716b8893a21d6a30a51c741df4eccde6683c1c15
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintSettings printSettings = new PrintSettings();
printSettings.documentConversionEnabled = true;

graphClient.customRequest("/print/settings", PrintSettings.class)
    .buildRequest()
    .patch(printSettings);

```