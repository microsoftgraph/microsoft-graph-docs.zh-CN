---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f9a9aa69fee43ea20159b43cb9a6f224b5d6060
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981440"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOff timeOff = graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest()
    .get();

```