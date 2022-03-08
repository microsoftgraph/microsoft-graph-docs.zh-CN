---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a940a084a4c9c910c03a7f9b627e794d155fa870
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351191"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Profile profile = graphClient.me().profile()
    .buildRequest()
    .expand("names($select=first,last),skills($select=displayName)")
    .get();

```