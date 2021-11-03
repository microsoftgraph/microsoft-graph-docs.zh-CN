---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bdabd28423916615931134f91e8fad99a0097a04788a4b32b802b3f494821832
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .unpublish()
    .buildRequest()
    .post();

```