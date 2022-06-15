---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9b10a88cf740acc88630ca3da7d7dd47b1aa2f6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095579"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .filter("identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'My B2C tenant')")
    .select("displayName,id")
    .get();

```