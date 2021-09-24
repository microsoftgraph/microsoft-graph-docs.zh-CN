---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c7ee9b3d2217c515945097a8e98191ebe8cf575821bcf1fec932f9ee809a889
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().cloudPCs("{id}")
    .reprovision()
    .buildRequest()
    .post();

```