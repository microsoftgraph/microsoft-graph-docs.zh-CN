---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1981b64a8e9bf261a8923fae6ec2c679563a2de28ed452e68ce5bae3c861c54f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c").teamwork().installedApps("ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=").chat()
    .buildRequest()
    .get();

```