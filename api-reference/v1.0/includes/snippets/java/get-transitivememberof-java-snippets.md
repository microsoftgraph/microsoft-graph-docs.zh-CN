---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c40b9c0afba1bd9c528bd9fb4012fb371896d0d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904295"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage transitiveMemberOf = graphClient.users("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```