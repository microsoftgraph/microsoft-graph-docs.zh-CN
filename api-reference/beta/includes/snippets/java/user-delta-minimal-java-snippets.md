---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14f07e6544ea5ddc068010b731c7deaa8073b722
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

UserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mobilePhone")
    .get();

```