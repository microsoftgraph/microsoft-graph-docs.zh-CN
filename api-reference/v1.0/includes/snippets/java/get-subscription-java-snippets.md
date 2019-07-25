---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51db8742dd9d77a14208f7b2e5a4b1c71d29f32d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890547"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.subscriptions("{id}")
    .buildRequest()
    .get();

```