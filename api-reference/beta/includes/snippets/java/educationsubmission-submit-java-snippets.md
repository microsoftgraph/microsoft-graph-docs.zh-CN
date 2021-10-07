---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11bd3b27a99a34a3dc4cd3b3c46889880cf835ccfe4f27768c44e35762716ae0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219551"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7")
    .submit()
    .buildRequest()
    .post();

```