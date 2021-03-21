---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8deef1c849a5a6fe06d99b5d1d03d21f1b249f20
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969123"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .get();

```