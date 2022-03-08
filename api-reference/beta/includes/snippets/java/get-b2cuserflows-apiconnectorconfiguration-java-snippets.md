---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b68cb53d99ef1cad828296a444d0d6ad40aeb5762201f575c68deef98cc734e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902864"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowApiConnectorConfiguration userFlowApiConnectorConfiguration = graphClient.customRequest("/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration", UserFlowApiConnectorConfiguration.class)
    .buildRequest()
    .get();

```