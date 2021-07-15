---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c510ddeb5a5020d4a481c5ef18cffcf58db69ee
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/odata/groups('dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef')"));

graphClient.policies().mobileDeviceManagementPolicies("dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef").includedGroups().references()
    .buildRequest()
    .post(group);

```