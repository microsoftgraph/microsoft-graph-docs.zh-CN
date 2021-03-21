---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdac918ca63ca4f34bbccbe786c212e3d479ce75
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983736"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.contacts("{id}")
    .buildRequest()
    .delete();

```