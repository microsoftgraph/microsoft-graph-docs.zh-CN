---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f87f481e54e1265014b5fa12b2ffb3ed7c1924d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61008170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)")
    .buildRequest()
    .get();

```