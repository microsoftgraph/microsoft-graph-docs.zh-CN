---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e956c4673b682bfa57ba7c60ffa24d27f5566454
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888337"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest()
    .get();

```