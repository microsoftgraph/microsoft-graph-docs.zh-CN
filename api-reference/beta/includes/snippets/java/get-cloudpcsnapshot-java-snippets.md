---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b485da7ff0f165c29439780536895caca86b4160
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333503"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcSnapshot cloudPcSnapshot = graphClient.deviceManagement().virtualEndpoint().snapshots("A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8")
    .buildRequest()
    .get();

```