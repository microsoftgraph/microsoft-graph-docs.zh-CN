---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0c3c045382afed9010c06c244971e7d1d08bc09
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966849"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content oauth2PermissionGrants = graphClient.users("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```