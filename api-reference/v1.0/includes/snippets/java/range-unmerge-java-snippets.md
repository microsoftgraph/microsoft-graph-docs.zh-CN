---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43415ad30a29388e73a73146c908cd38da6775e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967886"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .unmerge()
    .buildRequest()
    .post();

```