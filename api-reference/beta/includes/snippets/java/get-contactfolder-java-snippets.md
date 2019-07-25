---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f409916deba7e9dac02f1cb3b6d4db94417155e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = graphClient.me().contactFolders("{id}")
    .buildRequest()
    .get();

```