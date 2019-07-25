---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 73a262aef0843a78a98e1209e717da8b348045cf
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886508"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .delete();

```