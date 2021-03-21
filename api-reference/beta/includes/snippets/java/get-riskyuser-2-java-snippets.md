---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 356217c837be14ccc8d83da6cb4c63852af67c5d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960771"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskyUserCollectionPage riskyUsers = graphClient.identityProtection().riskyUsers()
    .buildRequest()
    .get();

```