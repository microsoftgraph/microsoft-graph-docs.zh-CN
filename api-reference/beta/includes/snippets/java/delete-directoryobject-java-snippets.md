---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf6f1fbc999e62c11a29b06c2600d8ff84495318
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972004"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryObjects("ffab4dce-9b82-49a6-b7c7-1a143106598c")
    .buildRequest()
    .delete();

```