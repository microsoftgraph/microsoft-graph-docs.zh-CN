---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 093824794883e4b2602d32186f689a702c7f48bd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest()
    .select("displayName,description,mailNickname")
    .get();

```