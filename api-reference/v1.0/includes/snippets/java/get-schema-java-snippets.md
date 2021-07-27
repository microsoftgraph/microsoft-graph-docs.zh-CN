---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b8e5dfdb9f8ef7d8d24b5e1a1c5b13890bc5834
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580668"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = graphClient.connections("contosohr").schema()
    .buildRequest()
    .get();

```