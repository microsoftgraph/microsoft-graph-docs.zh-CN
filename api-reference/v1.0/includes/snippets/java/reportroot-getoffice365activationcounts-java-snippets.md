---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 63b2fa5aadcda770bbddcfb8cf7c9c1c9bbd8933
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881078"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365ActivationCounts()
    .buildRequest()
    .get();

```