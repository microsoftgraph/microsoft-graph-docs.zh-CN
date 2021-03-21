---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e5522ce2225a7ec0be6b22457817c0e75fe92ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .removeFavorite()
    .buildRequest()
    .post();

```