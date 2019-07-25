---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f3d75e1c8ca7264be46422af6f7476b938947c3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895367"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactCollectionPage contacts = graphClient.me().contacts()
    .buildRequest()
    .select("displayName,emailAddresses")
    .get();

```