---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d614a390e8dc07d9b72e0ab0dadf19f827c6f53
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855064"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream Stream = graphClient.users("{id|userPrincipalName}").photo().content()
    .buildRequest()
    .get();

```