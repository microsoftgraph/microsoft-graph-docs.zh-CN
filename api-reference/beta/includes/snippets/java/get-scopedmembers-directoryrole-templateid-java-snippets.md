---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01edc7ebdf4bb061f0638f7737eb16123f99d9c908b228cf728a62e1503ac820
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278478"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScopedRoleMembershipCollectionPage scopedMembers = graphClient.directoryRoles("roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c").scopedMembers()
    .buildRequest()
    .get();

```