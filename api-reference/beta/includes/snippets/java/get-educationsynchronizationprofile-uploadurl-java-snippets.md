---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a540041b06d015f5037a047b18a5cf7c75456e6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String string = graphClient.education().synchronizationProfiles("{id}")
    .uploadUrl()
    .buildRequest()
    .get();

```