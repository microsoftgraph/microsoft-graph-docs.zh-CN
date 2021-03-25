---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a53d399f9b1e86408e10f19edad5d53c42ac44e6
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210304"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding()
    .buildRequest()
    .delete();

```