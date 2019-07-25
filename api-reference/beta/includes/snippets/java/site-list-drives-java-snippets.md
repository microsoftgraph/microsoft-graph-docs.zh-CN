---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 13bdf62b094c686e0d1b9cfd97a9a3f8dccac646
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861532"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveCollectionPage drives = graphClient.sites("{siteId}").drives()
    .buildRequest()
    .get();

```