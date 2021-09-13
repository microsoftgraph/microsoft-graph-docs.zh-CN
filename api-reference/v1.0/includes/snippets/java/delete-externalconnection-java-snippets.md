---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d77c72d859c94a8af12353e96128922e9ea58d8d27797415caa366c4827b52fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220427"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr")
    .buildRequest()
    .delete();

```