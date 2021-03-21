---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83b8dae79ce63ca1f44bea89f57d2d9e7227e7f9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983480"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11022")
    .buildRequest()
    .delete();

```