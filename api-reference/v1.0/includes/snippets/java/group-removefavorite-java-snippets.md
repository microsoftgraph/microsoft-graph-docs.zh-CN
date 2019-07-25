---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 84f40b63c3f48ecbba0a5134f0cef3d5b431b84a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885422"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .removeFavorite()
    .buildRequest()
    .post();

```