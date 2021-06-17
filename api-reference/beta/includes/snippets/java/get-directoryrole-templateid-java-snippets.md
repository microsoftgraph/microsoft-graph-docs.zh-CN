---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96b5ba3bdff1dca84059cce7e46e0de2fbd1c2c0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991743"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b")
    .buildRequest()
    .get();

```