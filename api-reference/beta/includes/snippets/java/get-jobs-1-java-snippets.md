---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 304b4c6168442d139265775be425dec085e588fd19875581ffe59ebc4fcc1268
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163106"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().printers("{id}").jobs()
    .buildRequest()
    .get();

```