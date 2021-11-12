---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1af97db2063e8f8c842969c057ab5ef2f175c228df5d6678fd297b42ed990684
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106703"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}")
    .restoreFactoryDefaults()
    .buildRequest()
    .post();

```