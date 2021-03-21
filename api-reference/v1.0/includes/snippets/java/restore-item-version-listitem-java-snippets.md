---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3875d2e390ca0dbedf047c7fc9f7731f86a81334
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972904"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions("{version-id}")
    .restoreVersion()
    .buildRequest()
    .post();

```