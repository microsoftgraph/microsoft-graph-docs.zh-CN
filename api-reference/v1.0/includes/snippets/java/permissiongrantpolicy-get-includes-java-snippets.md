---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b84f487d3f1b2cf01b436fa9554df4ef698ba8430c0d0f1a4f09e4219f0560ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219635"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PermissionGrantConditionSetCollectionPage includes = graphClient.policies().permissionGrantPolicies("microsoft-application-admin").includes()
    .buildRequest()
    .get();

```