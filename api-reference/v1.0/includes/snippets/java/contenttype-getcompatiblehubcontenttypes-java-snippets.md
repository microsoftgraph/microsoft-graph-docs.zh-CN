---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbe9ff62dad81e4c122af38f53512eed0dbed3f3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316098"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentTypeGetCompatibleHubContentTypesCollectionPage getCompatibleHubContentTypes = graphClient.sites("root").lists("Documents").contentTypes()
    .getCompatibleHubContentTypes()
    .buildRequest()
    .get();

```