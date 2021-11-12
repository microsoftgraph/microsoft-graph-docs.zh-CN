---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b90062b76490aa8b0200d4b0590f2ea91301036356995d136cc7d2a9295ff5c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218476"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

graphClient.me().outlook().tasks("AAMkADA1MT15rfAAA=")
    .complete()
    .buildRequest( requestOptions )
    .post();

```