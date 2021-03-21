---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb8d92190fa6e45deeeab24e2b59d7ec8c16d3a7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971680"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}").channels("{id}")
    .buildRequest()
    .delete();

```