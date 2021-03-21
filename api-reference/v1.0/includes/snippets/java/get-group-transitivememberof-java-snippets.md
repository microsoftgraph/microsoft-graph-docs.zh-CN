---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a609911270f35d3de8f09479d82071a5a6bd281c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975678"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.groups("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```