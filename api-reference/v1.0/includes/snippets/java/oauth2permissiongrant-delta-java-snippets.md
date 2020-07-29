---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b90e19a3045826058fea990a3a7f5ff897e52cf9
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509848"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = graphClient.oauth2permissiongrants("delta")
    .buildRequest()
    .get();

```