---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 751543acb2f6d82de257d3054039cce4b93ce6bb6e5bf5cc8eecaf79c9e13117
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .buildRequest()
    .delete();

```