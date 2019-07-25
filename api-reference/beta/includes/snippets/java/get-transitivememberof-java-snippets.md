---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f3eea4f49b7984de9952ce1ff5d5576c06a0ebe8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867042"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMemberOf = graphClient.me().transitiveMemberOf()
    .buildRequest()
    .get();

```