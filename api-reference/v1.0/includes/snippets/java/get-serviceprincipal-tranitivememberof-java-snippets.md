---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b85953e9a6568934e8c441e815637923dbc62f86
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905618"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMemberOf = graphClient.servicePrincipals("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```