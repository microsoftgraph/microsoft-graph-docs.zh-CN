---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb00ebf90988d518dbc789fb27dbe196cd343a5b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984252"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.me().messages("4aade2547798441eab5188a7a2436bc1").content()
    .buildRequest()
    .get();

```