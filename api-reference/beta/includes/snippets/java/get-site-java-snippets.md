---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bd51cc933f96ef4259068973a179dc40755c5f47b67c0d8fa9f1951b7a13cfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903741"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Site site = graphClient.sites("{site-id}")
    .buildRequest()
    .get();

```