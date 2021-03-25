---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbaec1a4fce2f3c1f854f43a791c556d1042e659
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209300"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .delete();

```