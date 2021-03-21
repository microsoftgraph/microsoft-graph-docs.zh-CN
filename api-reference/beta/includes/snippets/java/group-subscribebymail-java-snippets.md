---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e0997b1ec8e421e3a7b138f976cf97dbea4a2fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .subscribeByMail()
    .buildRequest()
    .post();

```