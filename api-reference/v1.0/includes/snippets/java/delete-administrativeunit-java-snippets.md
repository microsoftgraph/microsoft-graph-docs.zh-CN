---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11bc4d066ed3174d3f578054a57bdc591f5150211564e35f12ce61537bf6af59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279214"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .delete();

```