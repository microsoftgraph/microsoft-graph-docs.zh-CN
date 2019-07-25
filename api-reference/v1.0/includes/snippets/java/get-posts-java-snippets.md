---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ebe7df72d532e318f1b0bc1f8fbc8eef2849deaa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883610"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPostCollectionPage posts = graphClient.groups("{id}").threads("{id}").posts()
    .buildRequest()
    .get();

```