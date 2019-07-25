---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a57282327af55b470c402d61678e41460aa550d1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877124"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Stream> StreamList = new LinkedList<Stream>();
Stream Stream = new Stream();
Stream.target = "#para-id";
Stream.action = "insert";
Stream.position = "before";
Stream.content = "<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />";

StreamList.add(Stream);
Stream Stream1 = new Stream();
Stream1.target = "#list-id";
Stream1.action = "append";
Stream1.content = "<li>new-page-content</li>";

StreamList.add(Stream1);

graphClient.customRequest("/me/onenote/pages/{id}/content", Stream.class)
    .buildRequest()
    .patch(Stream);

```