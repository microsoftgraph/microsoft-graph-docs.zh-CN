---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 981da362503954fbc763265056a76beddafc4aadc5c58e012efa2fa324f68f03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219670"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .get();

```