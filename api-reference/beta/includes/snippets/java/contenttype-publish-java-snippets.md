---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 148f7f67b6fd68047f468701b879b69d4b9f5bffa4594546fbddad9b14f9cf35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278993"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .publish()
    .buildRequest()
    .post();

```