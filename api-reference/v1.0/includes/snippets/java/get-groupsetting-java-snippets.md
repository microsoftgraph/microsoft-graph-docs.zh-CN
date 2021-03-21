---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be1fc54e21988358b6dbd25c578135e115d6eae1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973347"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = graphClient.groupSettings("{id}")
    .buildRequest()
    .get();

```