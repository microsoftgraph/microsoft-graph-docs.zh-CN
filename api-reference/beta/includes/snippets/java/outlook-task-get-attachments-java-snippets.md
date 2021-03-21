---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44c17fe9e1d328b749675d91898383973278e9b6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.users("{id}").outlook().tasks("{id}").attachments()
    .buildRequest()
    .get();

```