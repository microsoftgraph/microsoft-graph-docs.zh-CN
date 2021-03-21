---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee89ed5586a477f65d11f5f5aabd055c53cafb44
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .get();

```