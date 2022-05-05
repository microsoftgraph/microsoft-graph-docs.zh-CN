---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf6f1fbc999e62c11a29b06c2600d8ff84495318
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220266"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryObjects("ffab4dce-9b82-49a6-b7c7-1a143106598c")
    .buildRequest()
    .delete();

```