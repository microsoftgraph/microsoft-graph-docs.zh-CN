---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14e7919b3ed828fb9ab16c4f2a7c1a4042517589
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971133"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().educationalActivities("{id}")
    .buildRequest()
    .delete();

```