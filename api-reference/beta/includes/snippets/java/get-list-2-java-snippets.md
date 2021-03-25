---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6177108af3ad3d8e76993844596cd0db15ba596f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209872"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-title}")
    .buildRequest()
    .get();

```