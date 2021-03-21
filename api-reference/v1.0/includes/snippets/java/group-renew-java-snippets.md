---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a9ee9f214a7fe2dbbfb8f8607cdcb618846aaf4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969013"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .renew()
    .buildRequest()
    .post();

```