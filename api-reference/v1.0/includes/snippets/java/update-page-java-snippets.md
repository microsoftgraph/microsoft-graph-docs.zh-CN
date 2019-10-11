---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5104df5940305ce1e699fe6a6b40de3bb50e0aa1
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428790"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Stream> streamList = new LinkedList<Stream>();
Stream stream = new Stream();
stream.target = "#para-id";
stream.action = "insert";
stream.position = "before";
stream.content = "<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />";

streamList.add(stream);
Stream stream1 = new Stream();
stream1.target = "#list-id";
stream1.action = "append";
stream1.content = "<li>new-page-content</li>";

streamList.add(stream1);

graphClient.customRequest("/me/onenote/pages/{id}/content", Stream.class)
    .buildRequest()
    .patch(stream);

```