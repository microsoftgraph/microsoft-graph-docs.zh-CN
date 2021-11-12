---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b7ef5605a59ad7d9019fad8e98007eb5055bbf3af8beae6ba2c02fc5f45e2ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278807"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage dailyPrintUsageByUser = graphClient.reports().dailyPrintUsageByUser()
    .buildRequest()
    .get();

```