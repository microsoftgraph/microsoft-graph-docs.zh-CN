---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81aae8d75808cd269e1ad1f573c7949df903fc80
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772098"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.print().printers("{printerId}").jobs("{printJobId}").documents("{printDocumentId}").content()
    .buildRequest()
    .get();

```