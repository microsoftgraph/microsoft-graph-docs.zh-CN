---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22c3b1dc6dcabdf5a880ad111108eda18a934147
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972652"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .cancel()
    .buildRequest()
    .post();

```