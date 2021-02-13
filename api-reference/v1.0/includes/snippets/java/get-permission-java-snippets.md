---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a130ae28fe564ebce5c37417ac9dee0c9ba2fd3f
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176868"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .get();

```