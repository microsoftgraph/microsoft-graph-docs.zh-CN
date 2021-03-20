---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbfb4872c5b46154bfa6dd1dd07ea5c05eec0c0f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968065"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .start()
    .buildRequest()
    .post();

```