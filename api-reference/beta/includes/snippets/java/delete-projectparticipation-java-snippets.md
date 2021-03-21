---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9f8fa19a2f9c8032b0d0143aeda08a402b8c745
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974548"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().projects("{id}")
    .buildRequest()
    .delete();

```