---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbb12b7f642596035c5af93dd4d04bfb521bbfe659ad9df2b8a5e4da41cbc43d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161200"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.users("{id}").outlook().tasks("{id}").attachments()
    .buildRequest()
    .get();

```