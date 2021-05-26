---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b764fb921e09632384ac7332b08e7c1450a5e367
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664770"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11012").assignments("19002").submissions("20302")
    .setUpResourcesFolder()
    .buildRequest()
    .post();

```