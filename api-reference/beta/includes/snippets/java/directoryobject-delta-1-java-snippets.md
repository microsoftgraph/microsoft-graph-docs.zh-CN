---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bed003c05d6101798b3805e066ad1f9a1f60778c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946637"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

DirectoryObject directoryObject = graphClient.directoryObjects("delta")
    .buildRequest( requestOptions )
    .get();

```