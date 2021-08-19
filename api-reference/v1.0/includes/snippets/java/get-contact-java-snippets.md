---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2de27b4a065e49003fa74e13cf18cdb349c882981c43765209567db6fb96ff23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332637"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = graphClient.me().contacts("{id}")
    .buildRequest()
    .get();

```