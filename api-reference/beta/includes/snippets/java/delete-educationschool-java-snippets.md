---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e966948c2ed46fe24e2750c56a546ca586d245e8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977597"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10002")
    .buildRequest()
    .delete();

```