---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eacc10081f4e39fcc66a91e8aa24ca2dcb0da96d
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719256"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectionQuota connectionQuota = graphClient.external().connections("contosohr").quota()
    .buildRequest()
    .get();

```