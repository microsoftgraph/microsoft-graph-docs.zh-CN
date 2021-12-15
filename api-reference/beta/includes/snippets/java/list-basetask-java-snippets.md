---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f283e6153ddc6155c854919888567d8ce9645b58
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525455"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content tasks = graphClient.me().tasks().lists().aQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm().tasks()
    .buildRequest()
    .get();

```