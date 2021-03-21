---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65e0d33f3e4ddba830c1045f03ea0497dc5ee56a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest()
    .delete();

```