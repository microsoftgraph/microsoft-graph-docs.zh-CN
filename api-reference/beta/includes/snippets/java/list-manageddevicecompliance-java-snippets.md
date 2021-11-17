---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd67f30c44cd3cc6bd8db34d8819c95d23c0031b7368bd7212b061f99361a6c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106132"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagedDeviceComplianceCollectionPage managedDeviceCompliances = graphClient.tenantRelationships().managedTenants().managedDeviceCompliances()
    .buildRequest()
    .get();

```