---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8edd4e2ffffab3fc8af95a44872f69075d52af8c55fafaa266af236d4693a6a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903297"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> messageIdsList = new LinkedList<String>();
messageIdsList.add("MC172851");
messageIdsList.add("MC167983");

graphClient.admin().serviceAnnouncement().messages()
    .archive(ServiceUpdateMessageArchiveParameterSet
        .newBuilder()
        .withMessageIds(messageIdsList)
        .build())
    .buildRequest()
    .post();

```