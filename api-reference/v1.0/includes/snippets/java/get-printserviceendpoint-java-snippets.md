---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3777076a0302d604635609ffb3efb8c3ca1b224d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972395"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceEndpoint printServiceEndpoint = graphClient.print().services("{printServiceId}").endpoints("{printServiceEndpointId}")
    .buildRequest()
    .get();

```