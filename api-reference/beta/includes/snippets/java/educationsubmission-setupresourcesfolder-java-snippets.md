---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b764fb921e09632384ac7332b08e7c1450a5e367
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52870113"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11012").assignments("19002").submissions("20302")
    .setUpResourcesFolder()
    .buildRequest()
    .post();

```