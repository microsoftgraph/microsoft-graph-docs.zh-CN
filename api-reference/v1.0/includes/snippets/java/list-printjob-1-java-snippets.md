---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aea107644be989e2e100da26d56e97ab815f7ef4112ce5b6ad6f01224debd0fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158412"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().printers("{printerId}").jobs()
    .buildRequest()
    .get();

```