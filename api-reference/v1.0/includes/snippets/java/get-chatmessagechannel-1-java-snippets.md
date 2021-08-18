---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c06902f3c6fa56eff21669dfccf20ca6741f8b60de3c7b4e9471b32993122e59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334137"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = graphClient.chats("19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces").messages("1612289992105")
    .buildRequest()
    .get();

```