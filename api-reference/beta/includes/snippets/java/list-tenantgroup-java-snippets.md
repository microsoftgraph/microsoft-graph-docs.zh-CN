---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c9f49cf15679435ec0b345dc0fb36b9a58452f9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440494"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantGroupCollectionPage tenantGroups = graphClient.tenantRelationships().managedTenants().tenantGroups()
    .buildRequest()
    .get();

```