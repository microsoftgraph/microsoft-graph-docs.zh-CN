---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c3d7490df410196e7363d576c49bbf08cdbb86c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983710"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOAuth2PermissionGrantCollectionWithReferencesPage oauth2PermissionGrants = graphClient.users("{id}").oauth2PermissionGrants()
    .buildRequest()
    .get();

```