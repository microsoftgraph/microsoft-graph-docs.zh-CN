---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6c5fc733b790d8ed64ee932616623c9d390d01c51d3099bfb1f02ba6c444d68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334066"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").delegatedPermissionClassifications("{id}")
    .buildRequest()
    .delete();

```