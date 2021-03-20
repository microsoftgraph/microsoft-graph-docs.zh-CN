---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5da2e9bc625f99b8110629ab3671ecc7a3004b6d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943728"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITodoTaskCollectionPage tasks = graphClient.me().todo().lists("35e2-35e2-721a-e235-1a72e2351a7").tasks()
    .buildRequest()
    .get();

```