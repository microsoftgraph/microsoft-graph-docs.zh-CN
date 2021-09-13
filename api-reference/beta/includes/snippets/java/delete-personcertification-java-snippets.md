---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18771391c1374940f4a6776875848e0544afbb64d061d2dfac6aca9273ca5afa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219126"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().certifications("{id}")
    .buildRequest()
    .delete();

```