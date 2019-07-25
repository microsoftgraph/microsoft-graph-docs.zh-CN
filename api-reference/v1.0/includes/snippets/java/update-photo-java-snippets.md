---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5dd4f5c842a3516627af2120206bfea6fdfb44b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856869"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfilePhoto profilePhoto = new ProfilePhoto();
profilePhoto.height = 99;
profilePhoto.width = 99;
profilePhoto.id = "id-value";

graphClient.users("{id|userPrincipalName}").photo()
    .buildRequest()
    .patch(profilePhoto);

```