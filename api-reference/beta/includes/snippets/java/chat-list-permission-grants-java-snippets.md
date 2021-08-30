---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 719a45af457fe18d1a4e1db69ed6c8863cd5ec75d60c569ed21857a2f3bf5723
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904265"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ResourceSpecificPermissionGrantCollectionPage permissionGrants = graphClient.chats("19:089ac694c48647c68035aae675cf78ab@thread.v2").permissionGrants()
    .buildRequest()
    .get();

```