---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04ea23b0eca7dcbf081a63ea06d1f5eb80ec988d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976348"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").jobs("{printJobId}")
    .start()
    .buildRequest()
    .post();

```