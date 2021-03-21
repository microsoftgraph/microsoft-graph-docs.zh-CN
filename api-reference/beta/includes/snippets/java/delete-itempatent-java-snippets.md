---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd1d06b720d88c70ccf1d1280b6996e3f0c66ad5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969702"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().patents("{id}")
    .buildRequest()
    .delete();

```