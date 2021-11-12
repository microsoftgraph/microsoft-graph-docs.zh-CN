---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50b9edadaf3d393b0e1b5f6de55a2a19dcf0b2a55f3b8c7a30317f440635d8f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104402"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.isRead = false;

graphClient.me().messages("{id}")
    .buildRequest()
    .patch(message);

```