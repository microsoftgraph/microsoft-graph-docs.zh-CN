---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4677ef089409e6ff7429bc2da273dbb8f40be64
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967231"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().interests("{id}")
    .buildRequest()
    .delete();

```