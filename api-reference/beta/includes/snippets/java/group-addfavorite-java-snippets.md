---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98cb2265485b829e11c59de1e79fe9acbc0c21fe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .addFavorite()
    .buildRequest()
    .post();

```