---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d2481aa7dd7099ec8020089c9f3de324dce35a81bd95d032b0025a5b92c4709
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162984"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().homeRealmDiscoveryPolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```