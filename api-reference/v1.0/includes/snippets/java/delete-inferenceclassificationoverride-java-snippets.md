---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bdc3716006221e9587a9250a84548e098e6ae35
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981346"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().inferenceClassification().overrides("98f5bdef-576a-404d-a2ea-07a3cf34af4r")
    .buildRequest()
    .delete();

```