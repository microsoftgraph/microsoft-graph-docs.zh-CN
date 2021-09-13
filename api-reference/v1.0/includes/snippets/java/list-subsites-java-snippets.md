---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22dc2617e1e27d6043ef8e630a325d9d24f3d5a1a1cec31ce02e2ebeed37aaa2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteCollectionPage sites = graphClient.sites("{site-id}").sites()
    .buildRequest()
    .get();

```