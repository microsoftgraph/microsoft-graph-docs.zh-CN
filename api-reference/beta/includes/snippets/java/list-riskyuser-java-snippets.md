---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e57ed6270a3fe1aec5014b214ceaf999f9fd60e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440823"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserCollectionPage riskyUsers = graphClient.tenantRelationships().managedTenants().riskyUsers()
    .buildRequest()
    .get();

```