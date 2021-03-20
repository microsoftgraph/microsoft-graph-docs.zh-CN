---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fea4f84e1bfbd41a60eb47d3aa882236ae0fcf4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947730"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.chats("{id}").messages("{id}").hostedContents("{id}").content()
    .buildRequest()
    .get();

```