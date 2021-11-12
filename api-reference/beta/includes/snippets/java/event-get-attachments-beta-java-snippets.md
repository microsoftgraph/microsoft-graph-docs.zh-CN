---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba0c3dae5a72ef7df8dc0b8a1710dbee9029bf3bccc209a08468f728075bf761
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332298"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentCollectionPage attachments = graphClient.me().events("{id}").attachments()
    .buildRequest()
    .get();

```