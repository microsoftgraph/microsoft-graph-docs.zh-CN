---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45343d919674a39b92f658834c52ab65c743e6c9117428805ea277fffe8bfa4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163978"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeCollectionPage userFlowAttributes = graphClient.identity().userFlowAttributes()
    .buildRequest()
    .get();

```