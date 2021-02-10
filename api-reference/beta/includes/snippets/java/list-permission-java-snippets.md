---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b345bcb0070c860718ef9014b070810c57956b6c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176469"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionCollectionPage permissions = graphClient.sites("{sitesId}").permissions()
    .buildRequest()
    .get();

```