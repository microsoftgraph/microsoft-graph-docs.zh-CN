---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a61fade0173cf574f21a1b7933d902724b9fc522383bac8bfd87945c31d4191
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().me().rubrics("{id}")
    .buildRequest()
    .delete();

```