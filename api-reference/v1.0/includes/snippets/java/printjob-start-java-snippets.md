---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13c57cd6d435063dd563576da02197837a2a09faaf4a493fee46882c7271a13e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162551"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").jobs("{printJobId}")
    .start()
    .buildRequest()
    .post();

```