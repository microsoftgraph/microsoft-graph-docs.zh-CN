---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2190deb61d4ecea7f336d2c9b006c09fa4951c64
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975151"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema().directories("{directoryId}")
    .discover()
    .buildRequest()
    .post();

```