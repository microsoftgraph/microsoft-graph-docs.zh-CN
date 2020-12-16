---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b1b62f53e28f368d99af249437cf6bd5cfa101e3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689475"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Chat chat = graphClient.users("f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c").teamwork().installedApps("ZjMyYjgzYmItNGZjOC00ZGI3LWI3ZjUtNzZjZGJiYjhhYTFjIyMyMmY3M2JiZS1mNjdhLTRkZWEtYmQ1NC01NGNhYzcxOGNiMmI=").chat()
    .buildRequest()
    .get();

```