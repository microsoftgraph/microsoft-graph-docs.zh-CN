---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f28a2a39e9fa0a8a9428bba86f5608e466c303a
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402086"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean across = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .merge(across)
    .buildRequest()
    .post();

```