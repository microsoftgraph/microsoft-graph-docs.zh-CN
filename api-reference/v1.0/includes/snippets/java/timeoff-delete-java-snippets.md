---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2effc42b61d2712f0b3d23d140a0bd418b87e035
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967899"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest()
    .delete();

```