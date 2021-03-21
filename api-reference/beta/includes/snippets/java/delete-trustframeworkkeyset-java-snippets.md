---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cb58595fe00485bda226ecdb88650a3ff6016d6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983188"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .delete();

```