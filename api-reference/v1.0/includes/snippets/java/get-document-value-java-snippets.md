---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc6cf4e600a2348f2a08df47fd9ac7faf82d1d777f7310177d03696a8e4a1fb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158421"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.print().printers("{printerId}").jobs("{printJobId}").documents("{printDocumentId}").content()
    .buildRequest()
    .get();

```