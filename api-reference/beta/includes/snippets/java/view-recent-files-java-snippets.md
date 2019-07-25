---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d2e578d1e89fd049d321bad6ee34f7e02373ce5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861503"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage recent = graphClient.me().drive()
    .recent()
    .buildRequest()
    .get();

```