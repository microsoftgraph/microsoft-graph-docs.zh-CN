---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcd8f5f8ff9e42a4257b04e662f13faca3ab4b74bfa86582cfd105243f92a817
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158368"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .get();

```