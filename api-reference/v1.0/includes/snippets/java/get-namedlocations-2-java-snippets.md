---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0cba473ca2ad24c7bdd490f8b3fb4e7bcf06945652b011b5a344c1873bbfed3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277251"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .filter("isof('microsoft.graph.ipNamedLocation')")
    .get();

```