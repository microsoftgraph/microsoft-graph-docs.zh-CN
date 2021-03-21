---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05deac778b3a0b0cbde3d57903a1081ebf53422
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967440"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

GroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,description,mailNickname")
    .get();

```