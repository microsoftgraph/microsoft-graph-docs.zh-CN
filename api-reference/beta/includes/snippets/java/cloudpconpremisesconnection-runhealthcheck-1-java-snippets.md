---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8498e24a9198bb91b351ceb7b48eee8473b4e1ed
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210375"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().cloudPCs("{id}")
    .reprovision()
    .buildRequest()
    .post();

```