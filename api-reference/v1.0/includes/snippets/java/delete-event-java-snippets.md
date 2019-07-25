---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc4de5926c35a25e7ebe73ddd74c96aab982938b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887459"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().events("{id}")
    .buildRequest()
    .delete();

```