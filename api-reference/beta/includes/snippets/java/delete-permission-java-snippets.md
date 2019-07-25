---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aee750c1a4d2c276bd66a8815055a96e681793d7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876997"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().items().{item-id}().permissions().{perm-id}()
    .buildRequest()
    .delete();

```