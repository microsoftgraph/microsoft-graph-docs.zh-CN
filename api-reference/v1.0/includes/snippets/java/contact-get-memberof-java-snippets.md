---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b53a710fef74c4122c9a96004782cd3714fb09253bd5ece38b60b6731357b8af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220983"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.contacts("{id}").memberOf()
    .buildRequest()
    .get();

```