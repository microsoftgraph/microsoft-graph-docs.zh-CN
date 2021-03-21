---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c51f91ce2f18a9917ac4bc3943cd331b9cf5c047
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982484"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.contacts("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```