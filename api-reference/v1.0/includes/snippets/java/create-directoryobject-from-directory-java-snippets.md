---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a956c4a2bf6c6820fc54f41e94a3d338fc5d0cf7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973520"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .restore()
    .buildRequest()
    .post();

```