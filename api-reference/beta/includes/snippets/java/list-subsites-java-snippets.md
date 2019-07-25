---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ec341925c5adaed5e1a48e1ae5bc269a5ed90f94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869658"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionPage sites = graphClient.sites("{site-id}").sites()
    .buildRequest()
    .get();

```