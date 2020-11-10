---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0fea4f84e1bfbd41a60eb47d3aa882236ae0fcf4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958099"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.chats("{id}").messages("{id}").hostedContents("{id}").content()
    .buildRequest()
    .get();

```