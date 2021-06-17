---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd716eb083167cbdb391bce418cbf90d9fd61072
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("fe8f10bf-c9c2-47eb-95cb-c26cc85f1830")
    .buildRequest()
    .get();

```