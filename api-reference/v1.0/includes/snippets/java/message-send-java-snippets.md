---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efb2781090f31c8fd0212eae2d419775e908beed
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884695"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .send()
    .buildRequest()
    .post();

```