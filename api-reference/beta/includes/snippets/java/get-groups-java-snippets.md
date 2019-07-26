---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7952b4528c31aef6dfd78f5b548642a22b81bcaa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858187"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .get();

```