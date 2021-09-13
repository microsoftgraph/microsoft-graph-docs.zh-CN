---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15165413e7718128a7744c24bdfce5857eac8e6cb1acdb693c03b148bd160761
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279730"
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