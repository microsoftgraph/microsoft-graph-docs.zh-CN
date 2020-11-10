---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 356217c837be14ccc8d83da6cb4c63852af67c5d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979158"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskyUserCollectionPage riskyUsers = graphClient.identityProtection().riskyUsers()
    .buildRequest()
    .get();

```