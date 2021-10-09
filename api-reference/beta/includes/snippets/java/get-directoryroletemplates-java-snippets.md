---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f32b6fee6aa90cab6bcff5a276035c81d5f8071cef613dae5484eb0204c613a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161736"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleTemplateCollectionPage directoryRoleTemplates = graphClient.directoryRoleTemplates()
    .buildRequest()
    .get();

```