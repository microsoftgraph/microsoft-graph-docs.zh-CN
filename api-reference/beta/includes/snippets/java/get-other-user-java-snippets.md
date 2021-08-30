---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c72f32df930dbf302bae38aa82a5da7c46b5e62f3241a6ba8b1d07a22ec1799
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218836"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{id}")
    .buildRequest()
    .get();

```