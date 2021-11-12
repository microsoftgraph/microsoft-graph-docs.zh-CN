---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 773f0d5283911b337f88fa9be9cd354a2201f7fefd24d0d6f277341d64666550
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}")
    .buildRequest()
    .delete();

```