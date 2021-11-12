---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 253ed6442d69026bfb0c4cd253e5aca686882ef7551d31bd97cbddee2f051b73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219530"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = new ItemEmail();
itemEmail.address = "Innocenty.Popov@adventureworks.com";

graphClient.me().profile().emails()
    .buildRequest()
    .post(itemEmail);

```