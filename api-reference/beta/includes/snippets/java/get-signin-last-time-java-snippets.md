---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dcfa4eba8de9b8eb83714efcefe1fa3db01d599e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953769"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .select("displayName,userPrincipalName,signInActivity")
    .get();

```