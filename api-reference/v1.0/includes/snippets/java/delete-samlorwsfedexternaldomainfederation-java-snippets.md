---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66ae7defd82d4d35b7f1f284e46b45735bb0d969
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315365"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().federationConfigurations("96db02e2-80c1-5555-bc3a-de92ffb8c5be")
    .buildRequest()
    .delete();

```