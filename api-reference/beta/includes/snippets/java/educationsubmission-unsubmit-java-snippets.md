---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21f6fe3b4dc3ffdfb9b9c41f91f1affc0b4641d8ad1b3b36ad65207a41f06e31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161264"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7")
    .unsubmit()
    .buildRequest()
    .post();

```