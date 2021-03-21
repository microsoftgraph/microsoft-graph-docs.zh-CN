---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cf9aad83a2985fdf5e3d4c813128f0161451219
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984321"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .buildRequest()
    .delete();

```