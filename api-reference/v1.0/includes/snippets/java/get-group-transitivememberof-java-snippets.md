---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6eeb0ca11ddf9c41f418bb82e36c2b6c593728c7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880942"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMemberOf = graphClient.groups("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```