---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5b4555836cd77c8167e551a2de17f6bdaeec51da8c9eb9a6d0ee415d7324c1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903064"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffReasonCollectionPage timeOffReasons = graphClient.teams("{teamId}").schedule().timeOffReasons()
    .buildRequest()
    .get();

```