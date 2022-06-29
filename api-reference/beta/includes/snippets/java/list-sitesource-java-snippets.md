---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2df423572127be2bef5282ddeb7090fbf5d8af0c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502741"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSourceCollectionPage siteSources = graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").custodians("0053a61a3b6c42738f7606791716a22a").siteSources()
    .buildRequest()
    .get();

```