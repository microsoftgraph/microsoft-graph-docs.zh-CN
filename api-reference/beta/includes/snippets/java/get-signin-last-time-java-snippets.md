---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2152d6bf8d5c67759c0caf66cc6ea75331758b7a9243d79780be5a5bbb54c5f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378556"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserCollectionPage users = graphClient.users()
    .buildRequest()
    .select("displayName,userPrincipalName,signInActivity")
    .get();

```