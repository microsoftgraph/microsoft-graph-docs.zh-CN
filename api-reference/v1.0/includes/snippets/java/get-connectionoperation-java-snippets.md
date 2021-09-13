---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0825a48ddad6fb6bfadd57f6f420f123e5317e8621bb7a3a65f2d26d350e39e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221423"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectionOperation connectionOperation = graphClient.connections("contosohr").operations("3ed1595a-4bae-43c2-acda-ef973e581323")
    .buildRequest()
    .get();

```