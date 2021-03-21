---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc3a4b67798cb94b2d86a02f2388340397a8ed91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973935"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteCollectionPage sites = graphClient.sites("{site-id}").sites()
    .buildRequest()
    .get();

```