---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae2fbc990557eb2aa5669f0dd71d85610b91d542
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980956"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("{organizationId}").settings().profileCardProperties("fax")
    .buildRequest()
    .delete();

```