---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81be720cdbbbd42b304c8776bc1a36ca06da1eb0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979049"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PostCollectionPage posts = graphClient.groups("{id}").threads("{id}").posts()
    .buildRequest()
    .get();

```