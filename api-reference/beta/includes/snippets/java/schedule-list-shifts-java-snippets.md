---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 370c27bd6341da435ea523f3ec6424c1a3cea5128bf9a068eee804a70f0c1490
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104728"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ShiftCollectionPage shifts = graphClient.teams("{teamId}").schedule().shifts()
    .buildRequest()
    .filter("sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z")
    .get();

```