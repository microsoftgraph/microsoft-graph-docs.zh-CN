---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce842097196fcd0c6691aa7be951185e92158a08ce173d1edabe98bf2bece5a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106053"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkAGUzY5QKgAAA=").attachments("AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=")
    .buildRequest()
    .get();

```