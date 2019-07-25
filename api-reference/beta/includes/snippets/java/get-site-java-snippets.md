---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a986eae6f9822af22d3c1964ac4e4173503e7c6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869671"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Site site = graphClient.sites("{site-id}")
    .buildRequest()
    .get();

```