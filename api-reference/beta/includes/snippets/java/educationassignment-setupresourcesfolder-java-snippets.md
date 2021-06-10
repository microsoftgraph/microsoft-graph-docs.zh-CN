---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b84f64320b7185444cdb2ee2c4ae062fa50ac28e
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11012").assignments("19002")
    .setUpResourcesFolder()
    .buildRequest()
    .post();

```