---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a0cbf66ebd9eeded79d43d818b19064f97e47b2
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610371"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessageHostedContentCollectionPage hostedContents = graphClient.chats("19:2da4c29f6d7041eca70b638b43d45437@thread.v2").messages("1615971548136").hostedContents()
    .buildRequest()
    .get();

```