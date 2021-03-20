---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b9eb3db38a3885c837a3e5eedbafe30cc2abe94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974111"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("46cc6179-19d0-473e-97ad-6ff84347bbbb")
    .restore()
    .buildRequest()
    .post();

```