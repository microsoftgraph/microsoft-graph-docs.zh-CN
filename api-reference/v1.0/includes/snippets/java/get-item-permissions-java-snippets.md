---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25faccfe2a32658f40607af48cf82136bb79b374
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888007"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionCollectionPage permissions = graphClient.me().drive().items("{item-id}").permissions()
    .buildRequest()
    .get();

```