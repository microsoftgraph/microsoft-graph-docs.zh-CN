---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f5c2fd2f0eab8d2ca31c3b3cda3f2b9a0884960
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905683"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionPage users = graphClient.users()
    .buildRequest()
    .select("displayName,userPrincipalName,signInActivity")
    .get();

```