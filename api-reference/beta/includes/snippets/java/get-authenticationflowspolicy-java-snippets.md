---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ed8b1a72e4286e9443cf206d7ce3c62aeb0aedb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974190"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationFlowsPolicy authenticationFlowsPolicy = graphClient.policies().authenticationFlowsPolicy()
    .buildRequest()
    .get();

```