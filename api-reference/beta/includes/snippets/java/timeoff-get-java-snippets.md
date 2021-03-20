---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d818f56cddad1c7840d91e37b068a7d79f144ca3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977840"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOff timeOff = graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest()
    .get();

```