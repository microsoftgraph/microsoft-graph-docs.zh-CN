---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23c667b25ee51cf5872923705300d757ab18535b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967397"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c").teamwork().installedApps("ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=").chat()
    .buildRequest()
    .get();

```