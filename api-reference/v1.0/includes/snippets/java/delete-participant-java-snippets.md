---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42072846460f1de1c763e63851c0140792428e40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979635"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").participants("{id}")
    .buildRequest()
    .delete();

```