---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a933971fc7cd7283db3e9852c4c825fa70ab9c0a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage transitiveMemberOf = graphClient.devices("{id}").transitiveMemberOf()
    .buildRequest()
    .get();

```