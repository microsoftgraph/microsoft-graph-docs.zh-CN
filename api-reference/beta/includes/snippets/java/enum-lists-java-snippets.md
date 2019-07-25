---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 34aab3d1def0aba64b2dabbf8a079827fed43d2b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880298"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IListCollectionPage lists = graphClient.sites("{site-id}").lists()
    .buildRequest()
    .get();

```